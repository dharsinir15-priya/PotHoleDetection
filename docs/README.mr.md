`# IPDS: बुद्धिमान रस्ते खड्डे शोध प्रणाली

## 30 सेकंदांत वापरून पहा

हार्डवेअर उपलब्ध नाही? काही हरकत नाही. तुमच्या गरजेनुसार खालील पर्याय निवडा:

| पर्याय | तुम्हाला काय मिळेल | आवश्यक हार्डवेअर |
|---|---|---|
| [Colab मध्ये उघडा](#) | नमुना प्रतिमा किंवा तुमच्या स्वतःच्या व्हिडिओवर खड्डे शोधणे आणि ट्रॅकिंग चालवा | काहीही नाही |
| Wokwi मध्ये सिम्युलेट करा | ESP32 सेन्सर नोड (MPU6050, NEO-6M GPS, DS3231) तुमच्या ब्राउझरमध्ये चालवा | काहीही नाही |
| `demo/app.py` | प्रतिमा आणि व्हिडिओंसाठी Gradio वेब UI (Hugging Face Space वर तैनात करता येते) | काहीही नाही |
| स्थानिक इन्स्टॉलेशन (खाली दिले आहे) | संपूर्ण प्रक्रिया: व्हिडिओवर ऑफलाइन किंवा ESP32 बोर्डसह थेट वापर | ऐच्छिक |


## स्थानिक पातळीवर जलद सुरुवात (Local quickstart)

```bash
git clone https://github.com/SanTiwari07/PotHoleDetection.git
cd PotHoleDetection
pip install -r requirements.txt

# Vision-only on any road video (weights auto-download on first run)
python python/main.py --source path/to/road_video.mp4
```

आउटपुट `outputs/videos/` मध्ये (अॅनोटेट केलेला MP4 व्हिडिओ) आणि `outputs/logs/` मध्ये (CSV फाइल) साठवले जातात. थांबवण्यासाठी `q` दाबा; सर्व्हरवर चालवत असल्यास `--no-display` जोडा.
