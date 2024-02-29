git clone https://github.com/Georgeclark04/dockertest.git
cd dockertest/pyth
sudo docker build -t dockertest .
sudo docker run -p 5000:8080 -tid dockertest
Browse to http://localhost:5000
