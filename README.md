import random

def get_user_input():
    """收集用户输入以个性化故事"""
    print("欢迎来到故事生成器！请回答以下问题来创建您的专属故事。")
    
    character = {
        'name': input("请输入主角的名字: "),
        'profession': input("请输入主角的职业(如巫师、骑士、侦探等): "),
        'trait': random.choice(['勇敢的', '聪明的', '幽默的', '神秘的', '善良的'])
    }
    
    setting = {
        'place': random.choice(['森林', '城堡', '太空船', '古墓', '现代城市']),
        'time': random.choice(['中世纪', '未来', '古代', '现代', '奇幻世界'])
    }
    
    conflict = random.choice([
        '寻找丢失的宝藏',
        '解开神秘谜题',
        '对抗邪恶势力',
        '拯救被绑架的亲人',
        '阻止世界末日'
    ])
    
    companion = {
        'name': random.choice(['会说话的猫', '机器人助手', '精灵向导', '退休的教授', '勇敢的骑士']),
        'trait': random.choice(['忠诚的', '聪明的', '幽默的', '勇敢的', '神秘的'])
    }
    
    return {
        'character': character,
        'setting': setting,
        'conflict': conflict,
        'companion': companion
    }
