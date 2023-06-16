# Copyright 2022 IBM Corporation
# 
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
# 
#     http://www.apache.org/licenses/LICENSE-2.0
# 
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

FROM ibm-zcon-server:3.0.70

# customise server.xml via dropins
COPY --chown=1001:0 src/main/liberty/config /config/configDropins/overrides

# install war
COPY --chown=1001:0 build/libs /config/dropins
