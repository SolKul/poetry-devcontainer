FROM python:3.12-bookworm

# Set environment
ENV TZ Asia/Tokyo
ENV LANG en_US.UTF-8
ENV LC_ALL en_US.UTF-8

# set locale
RUN DEBIAN_FRONTEND=noninteractive && \ 
apt-get update && apt-get install -y locales && \ 
apt-get clean && rm -rf /var/lib/apt/lists/* && \ 
printf '%s\n' LANG=en_US LC_ALL=en_US.UTF-8 >/etc/default/locale && \ 
echo en_US.UTF-8 UTF-8 >>/etc/locale.gen && \ 
locale-gen