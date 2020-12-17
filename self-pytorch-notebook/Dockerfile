FROM jupyter/datascience-notebook:281505737f8a
MAINTAINER likang "komlei122@163.com"
# 下面是按官网的方法安装spotlight
# RUN pip --no-cache-dir install --upgrade install http://download.pytorch.org/whl/cu75/torch-0.2.0.post3-cp36-cp36m-manylinux1_x86_64.whl 
# RUN pip --no-cache-dir install --upgrade torchvision

# pytorch
RUN conda install pytorch torchvision -c soumith
# spotlight(https://github.com/maciejkula/spotlight)
RUN conda install -c maciejkula -c soumith spotlight=0.1.2

EXPOSE 8888
USER jovyan
CMD ["start-notebook.sh"]