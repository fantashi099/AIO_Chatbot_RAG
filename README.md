# AIO - 2024: Project: Chatbot with RAG

## Personal Information

- Member: Tran Minh Tien
- ID: 018
- [Facebook: Minh Tiến](https://www.facebook.com/fantashi099)

## Project Information

### Instllation

`conda` virtual environment is recommend

```sh
conda create -n chatbot_rag python=3.10 && conda activate chatbot_rag
pip install -r requirements.txt
```

### Usage

This project can be tested in the Google Colab. Here are few step to run the project:

1. You need to create an account from `ngrok` to get the Authtoken that public port from server machine (google-colab). You can excess to the following link to get your token: [https://dashboard.ngrok.com/get-started/your-authtoken](https://dashboard.ngrok.com/get-started/your-authtoken)
2. Export the ngrok Authtoken:

You can export through terminal:

```sh
export NGROK_AUTHTOKEN=$YOUR_AUTHTOKEN
```

or you can uncommend and change the this line in code:

```python
os.environ['NGROK_AUTHTOKEN'] = "YOUR_AUTHTOKEN"
```

3. Run the project:

```sh
chainlit run app.py --host 0.0.0.0 --port 8000 & >/ content / logs . txt &
```