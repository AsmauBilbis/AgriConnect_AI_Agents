# AgriConnect AI Agent

Multi-Agent AI System for Agricultural Disease Diagnosis in Hausa

Empowering Nigerian Farmers with Instant, Accessible Crop Intelligence

---

## 🎯 Problem Statement

In Northern Nigeria, over 70% of the workforce depends on agriculture, yet farmers face devastating crop losses:

- 🔴 20-80% crop losses from diseases annually
- 🔴 No access to agricultural extension officers
- 🔴 Language barriers - existing AI tools only in English
- 🔴 Incomplete information - farmers lack integrated market and weather intelligence

**The result?** Billions of Naira in losses, food insecurity, and farmers unable to support their families.

---

## 💡 Solution

AgriConnect is a production-ready multi-agent AI system that provides:

- ✅ Instant disease diagnosis using Gemini Vision AI
- ✅ Complete Hausa translation for accessibility
- ✅ Market intelligence with real-time prices
- ✅ Weather forecasting for treatment timing
- ✅ Treatment recommendations with prevention strategies
- ✅ Farmer memory profiles for personalized advice

**Execution time:** 15-20 seconds for complete analysis

---

## 🏗️ System Architecture

Five specialized AI agents orchestrated to deliver comprehensive agricultural intelligence

### The Five Agents

| Agent | Role | Technology | Output |
|-------|------|------------|--------|
| 🔬 Crop Pathologist | Disease identification | Gemini Vision API + Disease DB | Disease name, severity, treatment |
| 📊 Quality Assessor | Plant health evaluation | Gemini Vision API | Health score (0-100), damage assessment |
| 🌍 Geo-Context | Market & weather intelligence | Weather API + Market data | Prices, forecast, advisories |
| 🌐 Translation | Hausa accessibility | Gemini API | Complete Hausa translation |
| 💾 Memory Bank | Personalization | Session management | Farmer profiles, history |

---

## ✨ Key Features

### 🎯 Core Capabilities

- **Multi-Agent Orchestration** - 5 specialized agents working in harmony
- **Vision AI** - Gemini Vision for accurate disease identification
- **Bilingual Support** - Full English + Hausa functionality
- **Comprehensive Intelligence** - Disease + Market + Weather in one report
- **Memory System** - Personalized recommendations based on farmer history
- **Production-Ready** - Error handling, quota management, observability

### 📊 Dataset

- **Total Images:** 20,188 labeled disease images
  - **Maize:** 4,188 images (Blight, Common Rust, Gray Leaf Spot, Healthy)
  - **Rice:** 16,000 images (Bacterial Leaf Blight, Brown Spot, Leaf Smut, Healthy)
- **Disease Conditions:** 8 comprehensive conditions
- **Knowledge Base:** Scientific names, symptoms, treatments, prevention, Hausa terminology

### 🌐 Accessibility

- **First Hausa-language agricultural AI** in Nigeria
- **50+ agricultural terms** translated accurately
- **Culturally adapted** terminology and recommendations
- **Mobile-friendly** interface design

---

## 🚀 Demo

### Live Example: Maize Farmer in Kano

**Input:**
```
📸 Image: Maize leaves with brown lesions
📍 Location: Kano, Nigeria
🌾 Crop: Maize
```

**Output (Hausa):**
```
RAHOTON GANO CUTA (Disease Report)

Cutar: Cutar Ganyen Masara ta Arewa (Northern Leaf Blight)
Tsanani: Mai Tsanani (Severe)
Makin Lafiya: 65/100

MAGANI (Treatment):
1. Yi amfani da Mancozeb fungicide
2. Fesa a lokacin farko na alamomi
3. Maimaita bayan kwana 7-14

RIGAKAFI (Prevention):
- Shuka nau'ukan da ke da juriya
- Kiyaye tazarar da ta dace
- Share ragowar amfanin gona

FARASHI A KASUWA (Market Prices):
Kano: ₦35,000/100kg
Kaduna: ₦33,500/100kg

HASASHEN YANAYI (Weather):
Yau: 32°C, Hazo mai yawa
Zango: Rana mai zafi, babu ruwan sama
```

**Impact:** Farmer applies treatment early, saves 50% of crop, earns ₦175,000+ (~$120 USD)

---

## 🛠️ Technology Stack

### AI & ML
- **Google Gemini 2.5 Flash** - Primary language model
- **Gemini Vision API** - Image analysis for disease detection
- **Gemini Translation API** - English to Hausa translation

### Framework & Tools
- **Google AI Agent Development Kit (ADK)** - Multi-agent orchestration
- **Python 3.10+** - Core programming language
- **Google Colab** - Development environment
- **Google Drive** - Dataset storage

### Libraries
- `google-genai` - Gemini API integration
- `PIL` - Image processing
- `pandas` - Data management
- `datetime` - Scheduling and timestamps

---

## 📦 Installation & Usage

### Prerequisites
```
Python 3.10+
Google Colab account
Google Gemini API key
```

### Quick Start

**1. Open in Google Colab:**
- Click "Open in Colab" badge above
- Or upload AgriConnect_Clean.ipynb to Colab

**2. Set up API Key:**
```python
# In Colab, add your Gemini API key to Secrets
# Or set environment variable
import os
os.environ['GOOGLE_API_KEY'] = 'your-api-key-here'
```

**3. Configure Dataset Paths:**
```python
# Update paths to your Google Drive
MAIZE_PATH = '/content/drive/MyDrive/AgriConnect_data/corn_or_maize/'
RICE_PATH = '/content/drive/MyDrive/AgriConnect_data/rice-leaf-desease/'
```

### Usage Examples

**Example 1: Image-Based Diagnosis**
```python
result = agriconnect_demo_hausa(
    user_input="path/to/crop_image.jpg",
    input_type='image',
    location="Kano"
)
```

**Example 2: Market Intelligence Only**
```python
result = agriconnect_demo_hausa(
    user_input="rice",
    input_type='text',
    location="Kaduna"
)
```

**Example 3: Weather Advisory**
```python
result = agriconnect_demo_hausa(
    user_input="weather",
    input_type='text',
    location="Sokoto"
)
```

---

## 🏆 Technical Achievements

This project demonstrates all **5 key concepts** from the AI Agents Intensive:

### ✅ 1. Multi-Agent System
- 5 specialized agents with clear role separation
- Coordinator agent for orchestration
- Parallel execution for efficiency

### ✅ 2. Tools Integration
- Gemini Vision API (2 uses: Pathologist + Quality Assessor)
- Gemini Translation API
- Custom Disease Knowledge Base
- Market data integration
- Weather forecasting

### ✅ 3. Sessions & Memory
- InMemoryRunner for session management
- Farmer profile storage
- Diagnosis history tracking
- Preference persistence

### ✅ 4. Context Engineering
- Efficient prompt design
- Single comprehensive translation (not piecemeal)
- Smart image routing to multiple agents
- Token optimization

### ✅ 5. Observability
- Complete execution logging
- Performance metrics tracking
- Quota management and monitoring
- Error handling and recovery

### 🎁 Bonus Features
- **Extensive Gemini Usage** - Vision + Translation APIs
- **Production-Ready** - Error handling, quota management
- **Real-World Impact** - Solves actual problem for millions

---

## 🤝 Contributing

This is a capstone project, but feedback and suggestions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

## 🙏 Acknowledgments

- **AI Agents Intensive** - Kaggle Competition
- **Google Gemini Team** - For powerful AI APIs
- **Agricultural Extension Officers** - Domain expertise
- **Nigerian Farmers** - Inspiration and real-world validation
- **Kaggle Community** - Support and resources

---

## 📞 Connect

- 💼 **LinkedIn** - Your LinkedIn profile
- 🐦 **Twitter/X** - Your Twitter handle
- 📧 **Email:** albilbis360@gmail.com

---

## ⭐ Star This Repository

If you find AgriConnect helpful or interesting, please consider giving it a star! ⭐

It helps others discover the project and shows your support for AI solutions in agriculture.

---

**Built with ❤️ for Nigerian Farmers**

*AI Agents Intensive Capstone Project | Track: Agents for Good*

**Powered by Google Gemini AI & Agent Development Kit**
