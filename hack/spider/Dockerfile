FROM python:2.7
RUN mkdir /root/code & mkdir /root/spider163
WORKDIR /root/code
ADD ./ /root/code/
ADD hack/spider/spider163.conf /root/spider163/spider163.conf
RUN pip install -i http://mirrors.aliyun.com/pypi/simple --trusted-host=mirrors.aliyun.com -r requirements.txt && python setup.py install && spider163 --help
CMD spider163 webserver


