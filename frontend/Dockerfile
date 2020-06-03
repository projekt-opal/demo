FROM node:13.3.0


RUN wget https://github.com/projekt-opal/web-ui/archive/2.0.1.tar.gz && \
tar -xzf 2.0.1.tar.gz

# Setting working directory. All the path will be relative to WORKDIR
WORKDIR web-ui-2.0.1

ARG BACKEND_ADDRESS

#set the backend address
RUN sed -i 's@^    baseURL:.*@    baseURL:'\'"$BACKEND_ADDRESS"\''@' webservice/axios-dataSets.js

# Installing dependencies
RUN npm install

# Building app
RUN npm run build

# Running the app
CMD [ "npm", "start" ]
