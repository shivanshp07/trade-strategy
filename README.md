# Trade Strategy

The **Trade Strategy** project simulates cryptocurrency arbitrage opportunities across different markets. It focuses on comparing the bid-ask spreads of different currency pairs to find potential profits through trading routes.

## **Key Features**

- **DepthManager**: Manages the order book for different markets (e.g., SOL-INR, USDT-INR) and provides methods to get the lowest ask price and the highest bid price.
- **Arbitrage Simulation**: Calculates potential arbitrage opportunities by checking if you can convert one asset into another and back profitably through a series of trades.
- **Order Creation and Cancellation**: Simulates placing and canceling orders using the `createOrder` and `cancelAll` functions.
- **Market Simulation**: Continuously updates potential arbitrage results and displays if it's profitable to move between currency pairs.

## **Technology Stack**

- **TypeScript**: Manages API requests and market data handling.
- **Axios**: Used for HTTP requests to interact with market data.
- **Crypto**: Handles secure API interactions.
- **Request**: Simplifies HTTP request handling.

## **How to Run**

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/trade-strategy.git
    ```

2. **Navigate to the project directory:**

    ```bash
    cd trade-strategy
    ```

3. **Install dependencies:**

    ```bash
    npm install
    ```

4. **Configure API Keys:**

    - Create a `config.ts` file in the `src` directory.
    - Add your API credentials:

    ```typescript
    export const key = "YOUR_API_KEY";
    export const secret = "YOUR_API_SECRET";
    ```

    *Ensure `config.ts` is listed in `.gitignore` to keep your credentials secure.*

5. **Run the script:**

    ```bash
    npm start
    ```

## **Usage**

The project continuously simulates trades and provides output on possible arbitrage gains based on current market prices. It places and cancels orders to mimic real trading behavior.

## **Sample Output**

