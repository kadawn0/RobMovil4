# Repo Turtlebot N°4 de 2000 USD
Repositorio de código par Turtlebot 4 - Robótica Móvil 2018-1

## Instrucciones de instalación de ROS Hydro en Ubuntu 12.04
**Login como Root (se necesita ser parte de los admin de este Ubuntu**
```sh
sudo -s
```
**Configurar archivo sources.list:**
```sh
$  sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu precise main" > /etc/apt/sources.list.d/ros-latest.list'
```
**Llaves (configuración para evitar recibir un paquete corrupto):**
```sh
wget http://packages.ros.org/ros.key -O - | sudo apt-key add -
```
**Actualizar paquetes del sistema:**
```sh
sudo apt-get update
```
**Desktop-Full Install: (Recomendada) :** ROS, rqt, rviz, bibliotecas genéricas, simuladores 2D/3D, navegación y percepción 2D/3D
```sh
sudo apt-get install ros-hydro-desktop-full
```
**Inicializar ROSdep**
```sh
sudo rosdep init
rosdep update
```
**Setup del entorno de ROS**
```sh
echo "source /opt/ros/hydro/setup.bash" >> ~/.bashrc
source ~/.bashrc
```
**Instalar ROSinstall**
```sh
sudo apt-get install python-rosinstall
```
