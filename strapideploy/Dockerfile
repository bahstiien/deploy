FROM strapi/base
WORKDIR /app
COPY ./package.json ./
RUN yarn install
COPY . .
ENV NODE_ENV production
RUN yarn build
EXPOSE 1337
CMD ["yarn", "start"]