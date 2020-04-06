# 12nanban-un2
docker file for 12-produce-un2 with nanban (for non-core layers of un_base)

# How to use
docker rmi 12nanban-un2  
git clone git@github.com:ubukawa/12nanban-un2  
cd 12nanban-un2  
docker build -t 12nanban-un2 .  
docker run -it --rm -v ${PWD}:/data 12nanban-un2  
 
cd 12-produce-un2  
vi config/default.hjson  
mkdir /data/mbtiles/un-sub   //mbtilesDir

rake // or node index.js or node index_africa.js  
