यह Android Studio/GitHub Actions के लिए source project है, compiled APK नहीं।
इस runtime में Android SDK/Gradle उपलब्ध नहीं है, इसलिए APK compile नहीं कर सका।

Build करने के लिए:
1. ZIP को extract करके GitHub पर नया repository बनाकर सभी files upload करें।
2. GitHub के Actions tab में Build Android APK workflow चलाएँ।
3. Workflow सफल होने पर Artifacts में StarkBetAnalyzer-debug-apk डाउनलोड करें।
4. APK Android फोन में install करें।

फोन पर:
- ऐप खोलें; Floating permission दें।
- Screen analysis शुरू करें; Android के screen capture prompt को स्वीकार करें।
- फिर StarkBet खोलें। Floating panel OCR से स्क्रीन पर दिख रहे digits दिखाएगा।
- ऐप बंद करने के लिए Analyzer बंद करें दबाएँ।

सीमाएँ:
यह शुरुआती OCR prototype है, अभी game-specific history extraction/recording या prediction model नहीं।
यह स्क्रीन पर दिख रहे unrelated digits (timer, ID, balance) भी पकड़ सकता है।
यह hidden server algorithm नहीं पढ़ता और random परिणाम की गारंटी से भविष्यवाणी नहीं करता।
कोई password, OTP या payment detail साझा न करें।
