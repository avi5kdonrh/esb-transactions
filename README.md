<!--

     Copyright 2005-2015 Red Hat, Inc.

     Red Hat licenses this file to you under the Apache License, version
     2.0 (the "License"); you may not use this file except in compliance
     with the License.  You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

     Unless required by applicable law or agreed to in writing, software
     distributed under the License is distributed on an "AS IS" BASIS,
     WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
     implied.  See the License for the specific language governing
     permissions and limitations under the License.

-->
# This project contains two modules:

1. Database Module: contains persistence.xml

2. Feature Module: contains all the features and bundles

To run this: 

1. mvn clean install

2. on fuse karaf console: 

feature:repo-add mvn:org.jboss.fuse.examples.transactions/features/6.3.0/xml/features

feature:install pre-bundle

feature:install mid-db

feature:install post-bundle
