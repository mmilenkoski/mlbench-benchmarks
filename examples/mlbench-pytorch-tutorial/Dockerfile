FROM mlbench/mlbench-pytorch-base:latest

RUN pip install mlbench-core==2.0.0

# The reference implementation and user defined implementations are placed here.
# ADD ./requirements.txt /requirements.txt
# RUN pip install --no-cache-dir -r /requirements.txt

RUN mkdir /codes
ADD ./train_dist.py /codes/train_dist.py

EXPOSE 29500

ENV PYTHONPATH /codes