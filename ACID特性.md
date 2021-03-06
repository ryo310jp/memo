## Atomicity(原子性)

トランザクション内の処理がすべて実行されるか、または全く実行されないことを保証する性質。

## Consistency(一貫性)

トランザクションによりデータの矛盾が生じず、整合性を満たすことを保証する性質。

## Isolation(独立性)

複数のトランザクションを同時に実行した場合と、順番に実行した場合の結果が等しくなることを保証する性質。通常は使用するデータにロックをかけることで直列化可能性を保証する。

## Durability(永続性)

トランザクション操作の完了通知をユーザが受けた時点で、以後システムに障害が発生しても失われないことを保証する性質。
多くのデータベース実装では、トランザクション操作を永続性記憶装置上にログとして記録し、システムに異常が発生したらそのログを用いて異常発生前の状態まで復旧することで永続性を実現している。(ジャーナリング)
