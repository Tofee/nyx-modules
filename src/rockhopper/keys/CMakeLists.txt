# @@@LICENSE
#
#      Copyright (c) 2010-2013 LG Electronics, Inc.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
# LICENSE@@@

if(${WEBOS_TARGET_MACHINE_IMPL} STREQUAL emulator)
	nyx_create_module(KeysMain keys_common.c emulator/keys.c)
elseif(${WEBOS_TARGET_MACHINE_IMPL} STREQUAL device)
	nyx_create_module(KeysMain keys_common.c device/keys.c)
endif()
