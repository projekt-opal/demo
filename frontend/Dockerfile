FROM node:13.3.0


RUN wget https://github.com/projekt-opal/web-ui/archive/1.0.0.tar.gz && \
tar -xzf 1.0.0.tar.gz

# Setting working directory. All the path will be relative to WORKDIR
WORKDIR web-ui-1.0.0


#set the backend address
RUN sed -i 's@^    baseURL:.*@    baseURL:'\'"$BACKEND_ADDRESS"\''@' webservice/axios-dataSets.js

# Installing dependencies
RUN npm install

# Building app
RUN npm run build

# Running the app
CMD [ "npm", "start" ]
