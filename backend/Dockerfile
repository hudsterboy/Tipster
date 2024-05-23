FROM node:lts-alpine
ENV NODE_ENV=production
WORKDIR /app
COPY backend/package.json ./
COPY backend/package-lock.json ./
RUN npm ci
COPY ./backend .
EXPOSE 3001
CMD ["npm", "start"]
