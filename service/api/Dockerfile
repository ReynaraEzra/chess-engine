FROM pytorch/pytorch:1.11.0-cuda11.3-cudnn8-devel

WORKDIR /api

RUN rm /etc/apt/sources.list.d/cuda.list

RUN rm /etc/apt/sources.list.d/nvidia-ml.list

RUN apt-get update 

RUN apt-get install git build-essential gcc -y

COPY requirements.txt ./

RUN pip install -r requirements.txt

COPY . ./

EXPOSE 9091

CMD [ "python", "main.py"]