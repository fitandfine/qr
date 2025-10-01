# QR Code Generator Web Application
## Author: Anup Chapain
## [Live Page](https://fitandfine.github.io/qr/)
## Overview

The QR Code Generator Web Application is a responsive, user-friendly tool that allows users to generate various types of QR codes directly from their web browsers. It supports QR codes for:

- Website URLs or plain text
- WiFi network credentials
- WhatsApp messages
- Phone calls
- SMS messages
- Email drafts

Built using HTML, CSS, and JavaScript, this application leverages the [QRCodeStyling](https://github.com/kozakdenys/qr-code-styling) library to create customizable QR codes with a modern and clean interface.

---

## Features

- **Multi-Type QR Code Generation**: Supports QR codes for URLs, WiFi, WhatsApp, phone calls, SMS, and emails.
- **Responsive Design**: Optimized for both desktop and mobile devices.
- **User-Friendly Interface**: Intuitive layout with clear instructions.
- **No Installation Required**: Fully functional directly in your web browser.
- **Customizable QR Codes**: Utilize the QRCodeStyling library for advanced customization.

---

## Technologies Used

- **HTML5**: Structure and content of the web page.
- **CSS3**: Styling and layout, ensuring responsiveness.
- **JavaScript**: Logic for QR code generation and dynamic content updates.
- **QRCodeStyling Library**: A powerful library for generating customizable QR codes.

---

## How It Works

### 1. User Interaction

Upon loading the application, users are presented with a dropdown menu to select the type of QR code they wish to generate. Depending on the selection, the relevant input fields are displayed:

- **URL/Text**: A single input field for the URL or text.
- **WiFi**: Fields for SSID, password, and encryption type.
- **WhatsApp**: Fields for phone number and message.
- **Call**: A field for the phone number.
- **SMS**: Fields for phone number and message.
- **Email**: Fields for recipient email, subject, and body.

### 2. 🔐 Data Handling and Privacy

Does this application store user data?

No, the QR Code Generator Web Application does not store any user data. All data entered by users—such as URLs, WiFi credentials, phone numbers, messages, or email content—is processed locally within the user's browser. Once the QR code is generated, the data is discarded and not retained by the application.

How does the application work?

- Local Processing: When a user selects a QR code type and enters the necessary information, the application constructs the appropriate data string (e.g., a URL, WiFi credentials, or a message).

- QR Code Generation: The data string is then used to generate a QR code using the QRCodeStyling library.

- Temporary Display: The generated QR code is displayed on the user's device for scanning.

- Data Disposal: After the QR code is generated and displayed, the application does not retain any of the entered data.

- No Data Transmission

- At no point does the application transmit any user data to external servers. All operations, including data processing and QR code generation, occur entirely within the user's browser.

#### Security Considerations

Since no data is stored or transmitted, the application poses minimal privacy risks. However, users should exercise caution when entering sensitive information, especially on shared or public devices.

### 3. QR Code Generation

Using the collected data, the application constructs the appropriate URL or string format for the selected QR code type. For example:

- **URL/Text**: Directly uses the input as the data.
- **WiFi**: Constructs a string like `WIFI:T:WPA;S:SSID;P:password;;`.
- **WhatsApp**: Constructs a URL like `https://wa.me/1234567890?text=Hello`.
- **Call**: Constructs a string like `tel:+1234567890`.
- **SMS**: Constructs a string like `SMSTO:+1234567890:Hello`.
- **Email**: Constructs a string like `mailto:email@example.com?subject=Subject&body=Body`.

### 4. QR Code Styling

The application utilizes the QRCodeStyling library to generate a QR code with the constructed data. The library allows for customization of:

- QR code size
- Dot type and color
- Background color
- Image overlays

### 5. Display

The generated QR code is displayed on the page, ready for scanning.

---

## How to Use

1. **Open the Application**: Launch the `index.html` file in your web browser.
2. **Select QR Code Type**: Use the dropdown menu to choose the type of QR code you want to generate.
3. **Enter Required Information**: Fill in the necessary fields based on your selection.
4. **Generate QR Code**: Click the "Generate QR Code" button to create and display the QR code.

---

## Customization

While the application currently does not support foreground and background color customization for the QR codes, the underlying QRCodeStyling library allows for extensive customization. Developers can modify the QRCodeStyling configuration in the `script.js` file to adjust:

- QR code size
- Dot type and color
- Background color
- Image overlays

For more information on customization options, refer to the [QRCodeStyling documentation](https://github.com/kozakdenys/qr-code-styling).

---

## Contributing

We welcome contributions to enhance the functionality and features of this project. To contribute:

1. Fork the repository.
2. Create a new branch for your changes.
3. Implement your changes and test thoroughly.
4. Submit a pull request detailing your changes and the reasoning behind them.

---

## License

This project is licensed under the MIT License - see the [LICENSE](https://en.wikipedia.org/wiki/MIT_License) file for details.

---

## Acknowledgments

- The [QRCodeStyling](https://github.com/kozakdenys/qr-code-styling) library for providing a robust solution for generating customizable QR codes.
- Open-source communities for their continuous contributions and support.

---

