# Technical assessment for Founding Developer - Full Stack Engineer

Thank you for your interest in our developer position. This assessment consists of two assignments that will help us evaluate your technical skills, problem-solving abilities, and coding practices.

## Timeline
- You have 72 hours from receiving this assignment to submit your solution
- Please submit your solution as a GitHub repository link

## Assignment 1: CEX/DEX Price Arbitrage Scanner

### Objective
Create a program that identifies arbitrage opportunities between Binance (CEX) and Solana DEX markets for USDC trading pairs.

### Requirements
1. Implement API integrations with:
   - Binance API for CEX price data
   - Solana blockchain for DEX price data

2. Core Functionality:
   - Scan and identify tokens that are traded against USDC on both platforms
   - Calculate real-time price differences accounting for all fees
   - Display only viable arbitrage opportunities (profitable after fees)

3. Fee Considerations:
   - Binance maker/taker fees
   - Solana DEX swap fees
   - Transaction costs on Solana

### Understanding Arbitrage
Arbitrage in cryptocurrency markets occurs when the same asset is priced differently across different exchanges. For example:
- If DOGE/USDC trades at $0.100 on Binance and $0.105 on Solana DEX
- Before concluding it's profitable, you must account for:
  - Binance fees (typically 0.1% maker/taker)
  - Solana swap fees (typically 0.3%)
  - Network transaction costs
  - Slippage and execution risk

## Assignment 2: Price Predictor with AI

### Objective
Develop an AI-powered price prediction system for cryptocurrency markets using Binance historical data.

### Requirements
1. Data Collection:
   - Integrate with Binance API to fetch historical price data
   - Implement proper data preprocessing and normalization

2. AI Implementation:
   - Choose and implement an appropriate AI algorithm for price prediction
   - Generate up/down predictions with probability percentages
   - Implement backtesting to validate the model

3. Backtesting Framework:
   - Test your prediction model against historical data
   - Calculate and display accuracy metrics
   - Visualize prediction performance

### Understanding Backtesting
Backtesting is a method to validate trading strategies using historical data. For example:
- If your model predicts BTC will go up in the next hour with 75% confidence
- Backtesting would apply this same prediction logic to past data
- Compare predictions against what actually happened
- Generate metrics like accuracy percentage, profit/loss if traded, etc.

### Suggested AI Approaches
You may consider these algorithms (not limited to):
- LSTM (Long Short-Term Memory) networks
- Random Forests
- Gradient Boosting Machines
- Support Vector Machines (SVM)
- Transformer-based models

## General Requirements for Both Assignments

### Frontend Implementation
- Create a web interface to display results
- Include relevant charts and visualizations
- Implement real-time updates where appropriate

### Repository Requirements
1. GitHub Repository:
   - Well-organized code structure
   - Clear documentation
   - Proper commit history

2. README.md must include:
   - Project overview
   - Installation instructions
   - Usage guide
   - Technical implementation details
   - API documentation if applicable
   - Development choices and rationale

### API Access Requirements
- Sign up for a Binance account at binance.com
- Create API keys through your Binance dashboard
- Store API keys securely and never commit them to the repository
- Use environment variables or secure configuration files for API credentials

### Development Guidelines
- You may use AI assistants (like Claude) for code generation
- Leveraging open-source libraries is encouraged (e.g., CCXT for exchange integration)
- Code quality and documentation are as important as functionality
- Consider scalability and maintainability in your design

### Recommended System Architecture Guidelines
While you're free to choose your own architecture, here are some recommended practices:

1. Real-time Data Handling:
   - Implement WebSocket connections for live price updates
   - Consider using a queuing system for managing multiple API requests
   - Include retry mechanisms for failed API calls
   - Implement rate limiting to comply with exchange API restrictions

2. Error Handling & Resilience:
   - Design fallback mechanisms for API outages
   - Implement circuit breakers for external service calls
   - Log errors comprehensively for debugging
   - Consider implementing automatic recovery procedures

3. Performance Optimization:
   - Use appropriate caching strategies for frequently accessed data
   - Consider implementing connection pooling for database operations
   - Optimize API calls to minimize latency
   - Consider batch processing where appropriate

These are suggestions to help you build a robust system, but you're welcome to implement alternative approaches if they better suit your solution.

### Evaluation Criteria
- Code quality and organization
- Problem-solving approach
- Documentation clarity
- Implementation of required features
- UI/UX design
- Error handling and edge cases

### Next Steps
- Submit your GitHub repository link when complete
- Be prepared for a follow-up interview where we'll discuss:
  - Your implementation choices
  - Potential improvements
  - Live coding modifications to enhance the solution

Good luck! If you have any questions about the requirements, please don't hesitate to ask for clarification.