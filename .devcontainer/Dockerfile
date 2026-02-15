FROM ubuntu:latest

RUN apt upgrade && apt update

RUN apt -y install python3 swi-prolog cmake curl build-essential git-all
RUN apt -y install python3-pip python3-tk

# RUN curl -d "action=AttachFile&do=get&target=fast-downward-23.06.tar.gz" -o fast-downward-23.06.tar.gz https://www.fast-downward.org/Releases/23.06 &&\
# tar -xvzf fast-downward-23.06.tar.gz &&\
# cd fast-downward-23.06 &&\
# ./build.py

RUN pip install mesa --break-system-packages
RUN pip install scikit-learn scipy matplotlib numpy seaborn bnlearn torch gpytorch "pgmpy==0.1.25" tqdm --break-system-packages
RUN pip install bnlearn --break-system-packages
RUN pip install ipykernel --break-system-packages