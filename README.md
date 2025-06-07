# -import random

def 模擬決勝時刻_城市交戰(玩家名稱: str, 城市: str):
    敵人數量 = random.randint(1, 5)
    成功擊殺 = 0
    print(f"{玩家名稱} 進入 {城市}，發現 {敵人數量} 名敵人。")

    for i in range(敵人數量):
        命中 = random.choice([True, False])
        if 命中:
            成功擊殺 += 1
            print(f"敵人 {i+1}：擊殺成功！")
        else:
            print(f"敵人 {i+1}：未擊中，敵人反擊！")

    print(f"{玩家名稱} 在 {城市} 中總共擊殺 {成功擊殺} 名敵人。")

# 使用範例
模擬決勝時刻_城市交戰("特戰兵阿強", "台北")
