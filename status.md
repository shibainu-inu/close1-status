# close-1 状況
更新: 09-26 08:23 JST

## 現在
- 審判: 最新 n=136（予定 09-26 08:20 JST、遅れ 14秒）、今の n=136、参照価格 225.18、登録済み owner 総数 837143（n=136）
- flow（n=1〜136）: 自分の取引 settled に見えた分 998件、void に見えた分 0件（どちらも一部しか載らない）
- ルールの repo: origin/HEAD=66c1da3（作業の基準 66c1da3）
- Issue/PR: 期間内の更新 9件（未解決 5）、コメント 13件
- 部屋: 登録用 50件、取引1 50件、取引2 50件、取引3 50件、取引4 50件
- 一括登録: 次の連番 6600、失敗 0件、停止中
- tree.py: 実行中、確定した取引 8243件。最新: n=136 区間1 ref=225.18 残りの脚 0 → 今回 0件（上限 1188）

## 最近の要確認（新しい順）
- 09-26 07:26 JST #5 に新しいコメント（2TheMoom）: Confirmed and fixed. Reproduced the exact minimal sequence from the report against `main` (`66c1da3`): the sweep-2 trade settles and its fee shows up in `sweeps`, while the already-returned `final` block still reports `fees: 0` and zero scores for both accounts. The two halves of the output do contradict each other, exactly as described.
- 09-26 07:23 JST flow n=74 で自分の取引が無効になっています（見えた分 1件）: [["rizzA-test-1790359503013", "limits"]]
- 09-26 07:23 JST flow n=38 で自分の取引が無効になっています（見えた分 2件）: [["test-double-1790348891", "settled"], ["test-double-1790348891", "settled"]]
- 09-26 06:52 JST 新しい Issue #9: Reference price frozen for 29 sweeps (22–50): ref stayed at 225.03 (13:49:57Z) while xyz:NVDA traded 223.34–225.71; 3,527 trades settled against it
- 09-26 06:31 JST #7 に新しいコメント（toma86hawk）: Confirmed the sweep-85 ranges from the export (thanks @kivica). One thing I tested before relying on them, in case it saves someone the same step: **the ranges are not predictable from the flow post alone.**
- 09-26 06:10 JST 取引2の部屋に自分以外の書き込み 1件
- 09-26 06:00 JST 取引1の部屋に自分以外の書き込み 1件
- 09-26 05:50 JST 取引4の部屋に自分以外の書き込み 1件
- 09-26 05:29 JST 取引3の部屋に自分以外の書き込み 1件
- 09-26 05:08 JST #7 に新しいコメント（kivica）: Correction to my own issue body, and one new observation.
- 09-26 03:45 JST 新しい Issue #8: close-1 after five hours: 598,644 owner keys, 3.7% hold a position, a 24-way tie at the top — a pre-seed footprint for close-2, and open tooling
- 09-26 03:35 JST #7 に新しいコメント（toma86hawk）: One correction to the thread, since it changes which of your two readings applies: **`missed` is not always empty.** Eight flow posts, all signed by the referee key (`…AAMzte`), list ranges in `close1` itself. Read from `/r/d-close1-flow/export` at 18:3xZ:
- 09-26 03:21 JST tree.py が止まっています
- 09-26 03:07 JST 登録用の部屋に自分以外の書き込み 65件
