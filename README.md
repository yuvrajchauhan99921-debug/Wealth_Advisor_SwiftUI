# Wealth_Advisor_SwiftUI
A macOS portfolio tracker built with SwiftUl that helps you manage your Indian stock market investments - with live price updates, SIP management, and an Al- powered financial advisor.
💰 WealthAdvisor
Your Personal Indian Stock Market Portfolio Tracker for macOS

WealthAdvisor is a native macOS portfolio tracking application built with SwiftUI. It helps you manage your Indian stock market investments, monitor portfolio performance, track Systematic Investment Plans (SIPs), and get AI-powered financial insights — all in one place.

✨ Features
📊 Portfolio Dashboard
View your total portfolio value and net worth.
Track overall profit and loss (P&L).
Visualize asset allocation with an interactive donut chart.
Get a consolidated overview of your investments.
📈 Live Stock Prices
Fetch live market prices for NSE and BSE-listed stocks.
Supports Yahoo Finance ticker symbols.
Examples: RELIANCE.NS, TCS.NS, INFY.NS.
🔍 Smart Ticker Search
Search for Indian stocks using ticker symbols.
Get ticker suggestions and autocomplete when adding assets.
Quickly find the stocks you want to track.
➕ Asset Management
Add, edit, and delete portfolio assets.
Track multiple asset categories:
Indian Stocks
Mutual Funds
Cash
Maintain investment quantities and average purchase prices.
📉 Asset Performance
View individual stock performance.
Explore historical price charts.
Monitor investment growth and price movements.
🔁 SIP Manager
Create and manage Systematic Investment Plans (SIPs).
Set monthly investment amounts.
Configure monthly deduction dates.
Track your recurring investments.
🤖 AI-Powered Financial Advisor
Integrated with Google Gemini 2.5 Flash.
Ask questions about your investment portfolio.
Get AI-generated insights based on your holdings.
Explore portfolio-related financial questions through an interactive chat interface.
📸 Portfolio Snapshots
Save snapshots of your portfolio at different points in time.
Compare historical portfolio values.
Track your investment journey over time.
🛠️ Tech Stack
Technology	Purpose
SwiftUI	Native macOS user interface
SwiftData	Local data persistence
Swift Charts	Interactive donut and performance charts
Google Generative AI SDK	Gemini 2.5 Flash integration
Yahoo Finance API	Stock price fetching
🚀 Getting Started

Follow these steps to set up and run WealthAdvisor locally.

Prerequisites

Make sure you have the following installed:

macOS 14 (Sonoma) or later
Xcode 15 or later
An active internet connection
A Google Gemini API key
1. Clone the Repository

Open Terminal and run:

bash
git clone git@github.com:Zenoop90/Wealth-Advisor.git


Navigate to the project directory:

bash
cd Wealth-Advisor

2. Configure Your Gemini API Key

To enable the AI Financial Advisor, you need a Gemini API key.

Visit Google AI Studio.
Generate your API key.
Open the following file in your project:

WealthAdvisor/AIAdvisorService.swift

Locate the API key placeholder:
swift
static let apiKey = "YOUR_GEMINI_API_KEY_HERE"

Replace the placeholder with your Gemini API key.
Security Note: Avoid committing API keys or other secrets to a public GitHub repository. For production use, store credentials securely rather than embedding them directly in the application.
3. Open the Project in Xcode

From the project directory, execute:

bash
open WealthAdvisor.xcodeproj


Alternatively, open WealthAdvisor.xcodeproj directly using Xcode.

4. Build and Run
Select your Mac as the run destination in Xcode.
Wait for the project to finish indexing.
Press ⌘ + R to build and run the application.

You're all set! 🎉

📂 Project Structure
text
WealthAdvisor/
│
├── WealthAdvisorApp.swift
├── ContentView.swift
│
├── DashboardView.swift
├── AdvisorView.swift
├── SIPManagerView.swift
├── AssetPerformanceView.swift
├── PerformanceChartView.swift
│
├── AddAssetView.swift
├── EditAssetView.swift
│
├── Asset.swift
├── SIP.swift
├── PortfolioSnapshot.swift
│
├── AIAdvisorService.swift
├── StockPriceService.swift
└── TickerSearchService.swift

Key Files
File	Description
WealthAdvisorApp.swift	Application entry point
ContentView.swift	Root navigation view
DashboardView.swift	Portfolio overview and asset allocation
AdvisorView.swift	AI financial advisor chat interface
SIPManagerView.swift	SIP creation and tracking
AssetPerformanceView.swift	Individual asset performance
PerformanceChartView.swift	Reusable chart components
AddAssetView.swift	Add new portfolio assets
EditAssetView.swift	Edit existing assets
Asset.swift	SwiftData asset model
SIP.swift	SwiftData SIP model
PortfolioSnapshot.swift	Portfolio snapshot model
AIAdvisorService.swift	Gemini AI integration
StockPriceService.swift	Live stock price fetching
TickerSearchService.swift	Stock ticker search and autocomplete
🔮 Future Improvements

Potential areas for future development include:

Advanced portfolio analytics and performance metrics.
Improved historical portfolio comparisons.
Enhanced stock discovery and filtering.
Additional investment insights and visualizations.
Secure API key management.
Support for additional investment categories.
⚠️ Disclaimer

WealthAdvisor is designed for personal investment tracking and educational purposes only.

The application and its AI-powered advisor do not provide certified financial, investment, or tax advice. AI-generated insights may be inaccurate or incomplete.

Always conduct your own research and consult a qualified financial advisor before making investment decisions.

📄 License

This project is licensed under the MIT License.

You are free to use, modify, distribute, and build upon this project in accordance with the license terms.

<div align="center">

💚 Built for Smarter Investing

WealthAdvisor — Track your investments. Understand your portfolio. Invest with confidence.

</div>
