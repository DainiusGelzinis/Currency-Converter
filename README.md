# Currency Converter

## Overview

Currency Converter is a desktop application built with Java Swing that allows users to convert between different currencies using live exchange rates from the Open Exchange Rates API. The application features a graphical user interface (GUI) for easy interaction and displays converted amounts to two decimal places.

## Features

- Convert between popular currencies including USD, EUR, GBP, CAD, AUD, and others.
- Uses live exchange rates fetched from Open Exchange Rates API.
- Simple and intuitive GUI built with Java Swing.
- Input validation for ensuring correct user input.
- Display converted amounts rounded to two decimal places.

## Technologies Used

- **Java (Swing)** for GUI components.
- **Open Exchange Rates API** for live currency rates.
- **Gson** library for parsing JSON data from the API.



## Usage

1. **Run the Application**:
   - You can run the project by launching the `CurrencyConverter` class through your IDE.

2. **Convert Currency**:
   - Enter the amount you want to convert.
   - Select the currency you are converting **from** and the currency you are converting **to**.
   - Click the **Convert** button to view the converted amount.

3. **Reset and Exit**:
   - Use the **Reset** button to clear all fields.
   - Use the **Exit** button to close the application.

## Code Overview

### Key Methods

- **`convertCurrency(double amount, String fromCurrency, String toCurrency)`**:
  - Converts the given amount from one currency to another using live rates fetched from the API.

- **`sendHttpRequest(String apiUrl)`**:
  - Sends an HTTP GET request to the API and returns the response as a JSON string.

### Main Components

- **GUI Components** (`initComponents()`):
  - The interface is built using Swing components such as `JPanel`, `JLabel`, `JButton`, and `JComboBox`.

- **Error Handling**:
  - The application includes input validation to ensure that the amount entered is numeric.
  - Catches and handles exceptions that may occur due to invalid API requests or network issues.
    
## Installation

### Prerequisites
- Java Development Kit (JDK) version 8 or above.
- An IDE that supports Java, such as NetBeans, IntelliJ, or Eclipse.
- Internet access to retrieve the latest currency rates.

### Getting Started

1. **Clone the Repository**:
   git clone https://github.com/yourusername/currency-converter.git
   cd currency-converter
   ```

2. **Open in Your IDE**:
   - Import the project into your favorite IDE (e.g., NetBeans, IntelliJ, Eclipse).

3. **Add Dependencies**:
   - Download and add the Gson `.jar` to your project. You can download it from [Gson GitHub repository](https://github.com/google/gson) or [Maven Central](https://mvnrepository.com/artifact/com.google.code.gson/gson).
   - Add it to your project by following your IDE's instructions to add external libraries.

4. **Set Up API Key**:
   - Sign up at [Open Exchange Rates](https://openexchangerates.org/) to get your API key.
   - Replace `"YOUR_API_KEY"` in the `CurrencyConverter` class with your actual API key.



Feel free to reach out with any questions or suggestions regarding this project.
