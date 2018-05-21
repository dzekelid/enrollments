---
name: Akamai
x-slug: akamai
description: Akamai Technologies, Inc. is a content delivery network or CDN and cloud
  services provider headquartered in Cambridge, Massachusetts, in the United States.
  Akamais content delivery network is one of the worlds largest distributed computing
  platforms, responsible for serving between 15 and 30 percent of all web traffic.
  The company operates a network of servers around the world and rents capacity on
  these servers to customers who want their websites to work faster by distributing
  content from locations close to the user
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Akamai_Technologies,_Inc._Logo.png
x-kinRank: "9"
x-alexaRank: ""
tags: Enrollments
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/enrollments/master/_listings/akamai/apis.md
specificationVersion: "0.14"
apis:
- name: Akamai API Create an Enrollment
  x-api-slug: akamai-api
  description: Create an Enrollment
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Akamai_Technologies,_Inc._Logo.png
  humanURL: https://akamai.com
  baseURL: https://developer.akamai.com////cps/v2/enrollments
  tags: Cps, Enrollments, Contract
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enrollments/master/_listings/akamai/cpsv2enrollments-post-openapi.md
- name: Akamai API List Enrollments
  x-api-slug: akamai-api
  description: List Enrollments
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Akamai_Technologies,_Inc._Logo.png
  humanURL: https://akamai.com
  baseURL: https://developer.akamai.com////cps/v2/enrollments
  tags: Cps, Enrollments, Contract
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enrollments/master/_listings/akamai/cpsv2enrollments-get-openapi.md
- name: Akamai API Get an Enrollment
  x-api-slug: akamai-api
  description: Get an Enrollment
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Akamai_Technologies,_Inc._Logo.png
  humanURL: https://akamai.com
  baseURL: https://developer.akamai.com////cps/v2/enrollments/{enrollmentId}
  tags: Cps, Enrollments, Enrollment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enrollments/master/_listings/akamai/cpsv2enrollmentsenrollmentid-get-openapi.md
- name: Akamai API Update an Enrollment
  x-api-slug: akamai-api
  description: Update an Enrollment
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Akamai_Technologies,_Inc._Logo.png
  humanURL: https://akamai.com
  baseURL: https://developer.akamai.com////cps/v2/enrollments/{enrollmentId}
  tags: Cps, Enrollments, Enrollment, Deploy, Not, Before,deploy, Not, After,allow,
    Cancel, Pending, Changes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enrollments/master/_listings/akamai/cpsv2enrollmentsenrollmentid-put-openapi.md
- name: Akamai API Delete an Enrollment
  x-api-slug: akamai-api
  description: Delete an Enrollment
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Akamai_Technologies,_Inc._Logo.png
  humanURL: https://akamai.com
  baseURL: https://developer.akamai.com////cps/v2/enrollments/{enrollmentId}
  tags: Cps, Enrollments, Enrollment, Deploy, Not, Before,deploy, Not, After,allow,
    Cancel, Pending, Changes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enrollments/master/_listings/akamai/cpsv2enrollmentsenrollmentid-delete-openapi.md
- name: Akamai API Get Change Status
  x-api-slug: akamai-api
  description: Get Change Status
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Akamai_Technologies,_Inc._Logo.png
  humanURL: https://akamai.com
  baseURL: https://developer.akamai.com////cps/v2/enrollments/{enrollmentId}/changes/{changeId}
  tags: Cps, Enrollments, Enrollment, Changes, Change
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enrollments/master/_listings/akamai/cpsv2enrollmentsenrollmentidchangeschangeid-get-openapi.md
- name: Akamai API Cancel a Change
  x-api-slug: akamai-api
  description: Cancel a Change
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Akamai_Technologies,_Inc._Logo.png
  humanURL: https://akamai.com
  baseURL: https://developer.akamai.com////cps/v2/enrollments/{enrollmentId}/changes/{changeId}
  tags: Cps, Enrollments, Enrollment, Changes, Change
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enrollments/master/_listings/akamai/cpsv2enrollmentsenrollmentidchangeschangeid-delete-openapi.md
- name: Akamai API Get a Certificate
  x-api-slug: akamai-api
  description: Get a Certificate
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Akamai_Technologies,_Inc._Logo.png
  humanURL: https://akamai.com
  baseURL: https://developer.akamai.com////cps/v2/enrollments/{enrollmentId}/deployments/production
  tags: Cps, Enrollments, Enrollment, Deployments, Production
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enrollments/master/_listings/akamai/cpsv2enrollmentsenrollmentiddeploymentsproduction-get-openapi.md
- name: Akamai API
  x-api-slug: akamai-api
  description: Akamai Technologies, Inc. is a content delivery network or CDN and
    cloud services provider headquartered in Cambridge, Massachusetts, in the United
    States. Akamais content delivery network is one of the worlds largest distributed
    computing platforms, responsible for serving between 15 and 30 percent of all
    web traffic. The company operates a network of servers around the world and rents
    capacity on these servers to customers who want their websites to work faster
    by distributing content from locations close to the user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Akamai_Technologies,_Inc._Logo.png
  humanURL: https://akamai.com
  baseURL: https://developer.akamai.com//
  tags: Enrollments
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/enrollments/master/_listings/akamai/openapi.md
x-common:
- type: x-base
  url: https://api.ccu.akamai.com
- type: x-blog
  url: https://blogs.akamai.com
- type: x-blog-rss
  url: http://blogs.akamai.com/feeds.html
- type: x-crunchbase
  url: http://www.crunchbase.com/company/akamai-technologies
- type: x-developer
  url: https://developer.akamai.com/
- type: x-email
  url: open-developer@akamai.com
- type: x-github
  url: https://github.com/akamai
- type: x-twitter
  url: https://twitter.com/Akamai
- type: x-website
  url: https://akamai.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---