Agregando a Jetson Nano
```nano ~/.bashrc

export CUDA_HOME=/usr/local/cuda 
export PATH=$CUDA_HOME/bin:$PATH 
export LD_LIBRARY_PATH=$CUDA_HOME/lib64:$LD_LIBRARY_PATH

export PYTHONPATH=/usr/lib/python3.6/dist-packages:$PYTHONPATH

export OPENBLAS_CORETYPE=CORTEXA57
```
Y CTRL + x, Y (de Yes) , Enter

Luego
`cd trt-models
chmod +X run.sh
./run.sh
`

Configuracion:
`config.env`
Cambiar datos como sea necesario

Corriendo:
`docker-compose up`


