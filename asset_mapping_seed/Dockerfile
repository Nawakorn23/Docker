# You don't need to modify the following 
FROM mongo:4.4

WORKDIR /var/dmongo
# copy initial data file to a directory in mongodb container
COPY profile_asset.json /var/dmongo
# run mongoimport
CMD mongoimport --host asset_mapping -d user -c userProfile --drop --type json --file /var/dmongo/profile_asset.json --jsonArray
