# -NO-1
import random
#ボールを設定する
Bingo_balls=[i for i in range(1,76)]
random.shuffle(Bingo_balls)
AppearedBalls=[]
#ボールの抽選
while Bingo_balls:
  lottery=input("ボールの抽選を始めますEnterを押してください。！※中止する場合はstopを入力！")
  if lottery=="stop":
    print("これでビンゴは終了です！")
    break
  Bingo_ball=Bingo_balls.pop()
  AppearedBalls.append(Bingo_ball)
  print(Bingo_ball,"の数字のボールが出ました！")
  print(f"今までの出目は{AppearedBalls}です")