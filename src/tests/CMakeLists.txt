# @@@LICENSE
#
#      Copyright (c) 2010-2013 Hewlett-Packard Development Company, L.P.
#                (c) 2013 Simon Busch <morphis@gravedo.de>
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

add_executable(nyx-test-ledcontroller test-ledcontroller.c)
target_link_libraries(nyx-test-ledcontroller ${GLIB2_LDFLAGS} ${GIO_LDFLAGS} ${NYXLIB_LDFLAGS})
webos_build_program(NAME nyx-test-ledcontroller)
