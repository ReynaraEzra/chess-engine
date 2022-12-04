FROM python:3.7
ENV TZ=Asia/Jakarta

WORKDIR /app

COPY requirements.txt .
RUN pip install -r requirements.txt

ADD . .

EXPOSE 3000
CMD ["python", "ChessMain.py"]