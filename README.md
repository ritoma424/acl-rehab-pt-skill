# 🦵 ACL Rehab Expert PT Skill

A structured AI-powered rehabilitation assistant designed for **ACL reconstruction recovery**, especially for complex cases involving:

* ACL reconstruction (hamstring graft)
* Meniscus repair (including posterior root repair)
* Notchplasty
* Multi-procedure knee surgeries

This skill turns LLMs (e.g. Claude) into a **professional-level physical therapist assistant**, providing:

* 📊 Recovery stage assessment
* 🏋️ Training plan evaluation
* ⚠️ Risk detection (meniscus / graft / swelling)
* 🧠 Personalized rehab adjustments
* 📈 Progress scoring

---

## 🚀 Features

* ✅ Persistent patient context (initialized once, reused forever)
* ✅ Structured JSON input/output
* ✅ Risk-first decision logic (meniscus root > ACL progression)
* ✅ Clinical reasoning (not generic advice)
* ✅ Daily rehab tracking support

---

## 🧠 How It Works

### 1️⃣ Initialize Patient Context (First Use)

```json
{
  "术后天数": 212,
  "手术详情": {
    "前交叉韧带": "自体腘绳肌腱 + 高强线带增强",
    "内侧半月板": "成型",
    "外侧半月板后根": "穿骨道+纽扣钛板固定",
    "髁间窝成型": true
  },
  "风险标记": [
    "半月板后根修复",
    "ACL移植物成熟期",
    "髁间窝撞击风险"
  ]
}
```

---

### 2️⃣ Daily Rehab Input

```json
{
  "术后天数": 220,
  "训练计划": [
    {
      "动作": "深蹲",
      "负重": "60kg",
      "组数": 4,
      "次数": 8
    }
  ],
  "症状反馈": {
    "疼痛": [
      {
        "位置": "膝前侧",
        "程度": 2,
        "类型": "酸痛"
      }
    ],
    "肿胀": false,
    "皮温升高": false,
    "不稳定感": false
  },
  "功能表现": {
    "走路": "正常",
    "单腿站立秒数": 30
  }
}
```

---

## 📊 Output Structure

The AI will respond with:

1. Recovery stage assessment
2. Training evaluation (✅ ⚠️ ❌)
3. Personalized rehab prescription
4. Pain & risk classification (🟢 🟡 🔴)
5. Recovery score (0–100)
6. Forbidden movements
7. Next-step priorities

---

## ⚠️ Disclaimer

This project is **NOT a medical diagnosis tool**.
It is designed for **educational and self-tracking purposes only**.

Always consult a licensed medical professional for:

* Severe pain
* Swelling
* Instability
* Suspected re-injury

---

## 🧩 Use Cases

* ACL post-op patients tracking rehab
* Physical therapy assistants
* Sports rehab enthusiasts
* AI + healthcare experimentation

---

## 📌 Roadmap

* [ ] Return-to-sport readiness module
* [ ] Symmetry scoring (left vs right)
* [ ] Rehab progression timeline tracking
* [ ] Visualization dashboard

---

## 🤝 Contributing

Feel free to open issues or submit PRs to improve:

* Rehab logic
* Risk detection
* Training templates

---

## 📄 License

MIT License
