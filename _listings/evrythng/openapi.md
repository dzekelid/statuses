swagger: "2.0"
x-collection-name: EVRYTHNG
x-complete: 1
info:
  title: EVRYTHNG
  description: the-evrythng-platform-is-a-cloud-platformasaservice-paas-for-storing-sharing-and-analyzing-data-generated-by-physical-objects--the-platform-gives-a-unique-and-permanent-digital-identity-also-known-as-adis-to-each-individual-object-and-allows-authorized-applications-and-users-to-access-it-via-rest-and-pubsub-mqtt-apis--visualisations-in-the-evrythng-dashboard-analytics-conditional-redirections-and-the-reactor-rules-engine-provide-means-to-add-intelligent-behavior-and-features-on-top-of-your-data-to-add-value-
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{USER_ID}/status:
    get:
      summary: /users/{id}/status (O)
      description: OPERATOR gets the status of a specific user.
      operationId: UsersStatusByUSERIDGet
      x-api-path-slug: usersuser-idstatus-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: USER_ID
      responses:
        200:
          description: OK
      tags:
      - Users
      - USER
      - ID
      - Status