FROM mongo:latest

MAINTAINER Johnny RAHAJARISON <johnny.rahajarison@mylittleadventure.com>

#COPY mongo.conf /usr/local/etc/mongo/mongo.conf

VOLUME /data/db /data/configdb

# CMD ["mongod"]

# # Connect to mongo and create admin user:
# # mongo
# use admin
# db.createUser(
#   {
#     user: "mlaAdmin",
#     pwd: "YA^e-cbLW33m^?JU",
#     roles: [ { role: "userAdminAnyDatabase", db: "admin" } ]
#   }
# )
# # Then, launch with auth
CMD ["mongod", "--auth"]

# Connect to mongo in admin user
# mongo -u mlaAdmin -p --authenticationDatabase "admin"
# use admin
# db.createUser(
#   {
#     user: "stats_clients",
#     pwd: "stats_clients",
#     roles: [
#        { role: "dbOwner", db: "stats_clients" },
#     ]
#   }
# )

EXPOSE 27017
