# voltcast-Hackathon
VoltCast predicts solar/wind availability using weather data and recommends the best time to run appliances. By applying Demand Response and Load Shifting, it reduces grid stress, improves renewable usage, and enables smarter, efficient energy consumption.
VoltCast is an AI-powered system that predicts renewable energy availability and optimizes electricity usage by recommending the best time to run high-power appliances.

It tackles the Duck Curve problem by aligning consumption with renewable generation using Load Shifting and Demand Response.

🚀 Features
🌤️ Weather-based solar prediction
🤖 Smart appliance scheduling
⚡ Real-time usage recommendations
📊 Simple dashboard (Flask UI)
🔌 Optional ESP32 + relay automation
🧠 How It Works
Weather API → Solar Prediction → Decision Engine → User Suggestion → (Optional) Relay Control
Fetch weather data
Predict solar availability
Decide optimal usage time
Display recommendation
(Optional) Control appliances
🛠️ Tech Stack
Python (Flask, Scikit-learn)
OpenWeather API
HTML/CSS
ESP32 + Relay Module
📁 Project Structure
VoltCast/
│── app.py
│── model.py
│── requirements.txt
│── templates/
│     └── index.html
│── esp32_code/
│     └── voltcast.ino
│── README.md
⚙️ Installation & Setup
1. Clone the repository
git clone https://github.com/your-username/VoltCast.git
cd VoltCast
2. Install dependencies
pip install -r requirements.txt
3. Add your API key

In model.py:

API_KEY = "YOUR_OPENWEATHER_API_KEY"
4. Run the app
python app.py

Open in browser:

http://127.0.0.1:5000/
🔌 ESP32 Integration (Optional)
Connect relay module to ESP32
Update WiFi credentials in voltcast.ino
Set your PC IP in API endpoint

ESP32 will:

Fetch /status from Flask server
Turn ON/OFF appliance based on solar prediction
🎯 Problem Statement

Renewable energy sources are intermittent, causing mismatch between generation and demand. This leads to inefficiencies and grid instability.

💡 Solution

VoltCast shifts energy consumption to periods of high renewable availability using AI-based prediction and scheduling.

🏆 Why VoltCast?
Focuses on consumption optimization
Easy to deploy in households
Scalable and cost-effective
Practical solution for smart grids
🔮 Future Scope
Advanced ML models (LSTM)
Real-time electricity pricing
Mobile app integration
Smart home ecosystem support
👨‍💻 Team
Voltcast
⭐ Demo Pitch (1 line)

“VoltCast intelligently schedules electricity usage based on renewable availability to reduce grid stress and improve efficiency.”
