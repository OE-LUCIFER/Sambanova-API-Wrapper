# Sambanova API Wrapper 🌟✨

Welcome to the Sambanova API Wrapper! 🎉 This Python script provides a simple way to interact with the Sambanova AI API for Free.

## Prerequisites 🛠️

Before you begin, make sure you have the following:

1. **Python** installed on your machine. 🐍
2. **Required Packages:** Install the necessary Python packages using pip:

```bash
pip install requests fake-useragent
```

3. Install the **Cookie-Editor** extension for either Chrome or Edge:
   - [Chrome Extension](https://chrome.google.com/webstore/detail/cookie-editor/...)
   - [Edge Extension](https://microsoftedge.microsoft.com/addons/detail/cookie-editor/...)

### Exporting Cookies 🍪

Once you have the Cookie-Editor installed, follow these steps to export your cookies:

1. Open the website from which you want to extract cookies. 🌐
2. Click on the Cookie-Editor extension icon. 🔍
3. Click the "Export" button to save your cookies in JSON format. 💾
4. Create a file in your working directory named `cookies.json`. 🗂️
5. Paste the data copied from the Cookie-Editor into `cookies.json` and save it. ✨

## Usage Limits 📊

Please note that usage limits for the Sambanova API are not publicly documented. Be mindful of your usage to avoid potential restrictions. 🚦

## Example Usage 💻💖

Let's explore some examples of how to use the Sambanova API Wrapper! 🎈

### Simple Prompt Example

```python
api = SambanovaAPI('cookie.json', model='Meta-Llama-3.2-1B-Instruct', system_prompt="You are a helpful assistant.")
for response in api.ask("What is the capital of France?"):
    print(response, end="", flush=True)
```

### Custom Model and System Prompt

```python
api = SambanovaAPI('cookie.json', model='Meta-Llama-3.1-70B-Instruct', system_prompt="You are a knowledgeable expert on 19th-century literature.")
for response in api.ask("Discuss the themes of realism in the novels of Gustave Flaubert."):
    print(response, end="", flush=True)
```


## Contributing 🤝💕

Contributions are welcome!  If you have suggestions or improvements, feel free to open an issue or submit a pull request.

## License 📄

This project is licensed under the MIT License

---

Thank you for using the Sambanova API Wrapper! We hope you find it helpful and enjoyable! Happy coding! 🎊💖
