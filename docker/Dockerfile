FROM node:16

COPY work /work

WORKDIR /work

RUN yarn cache clean

RUN yarn add graphql  @graphql-mesh/cache @graphql-mesh/runtime @graphql-mesh/cli @graphql-mesh/openapi @graphql-mesh/graphql 

CMD if [ -f "init.sh" ]; then sh init.sh; fi && yarn start


# docker build -t grape-vine . 
# docker run -e DEBUG=1 -p 4000:4000 grape-vine
