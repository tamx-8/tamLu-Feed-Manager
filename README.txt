tamLu Feed Manager v0.2
========================

Contents
- index.html: web app
- manifest.json: installable web app metadata
- sw.js: basic offline cache support

Try locally
1. Extract the ZIP.
2. Open index.html in a modern browser.

Publish online
Upload the extracted folder contents to a static hosting service that supports HTTPS
(for example, GitHub Pages, Netlify, or Cloudflare Pages). Upload the files themselves,
not just the ZIP, unless the hosting service explicitly accepts ZIP deployment.

Features
- Four herd groups
- Shared per-head feed amount
- Per-group herd and feeding head counts
- Auto-calculated kilograms and ratio gauges
- Gauge color: blue <= 90%, green > 90% and < 110%, red >= 110%
- Gauge scale 0–130%, with 100% marker
- Per-round task checklist
- Automatically saves settings and checklist in this browser using localStorage
- Removed the sample-value reset button

Prototype limitations
- No accounts or employee-to-employee cloud sync yet.
- Saved data stays in this browser on this device; it does not sync between employees or devices. Clearing browser data may erase it.
- Sample numbers are demo values; verify all amounts before operational use.


v0.5 変更点:
- 「作業確認」ページを削除し、「ミキサー」ページを追加
- 1,2回目の各群給餌量を1日必要量の約3分の1に近い500kg単位で自動計算
- 3回目は1日必要量から1,2回目の2回分を引いた残量を表示
- 3回分の合計が各群の1日必要量と一致
- Service Workerのキャッシュ更新方式を改善


v0.5の追加機能：ミキサー画面で▲▼ボタンにより給餌順を変更できます。順番は端末内に保存されます。各群の給餌後のミキサー残量は、選択中の回の全群給餌量合計から順番に差し引いて表示します。


v0.5の変更点：ミキサー画面の初期表示順を現場の給餌順「C群→D群→B群→A群」に変更しました。画面の▲▼ボタンで順番を変更することもできます。
