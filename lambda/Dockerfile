FROM public.ecr.aws/lambda/nodejs:18
COPY package.json /var/task/
COPY proxy.js /var/task/
COPY proxy-urls.json /var/task/
RUN npm install
CMD [ "proxy.lambdaHandler" ]
