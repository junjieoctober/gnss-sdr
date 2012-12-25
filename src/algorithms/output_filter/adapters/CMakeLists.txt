# Copyright (C) 2012-2013  (see AUTHORS file for a list of contributors)
#
# This file is part of GNSS-SDR.
#
# GNSS-SDR is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# at your option) any later version.
#
# GNSS-SDR is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with GNSS-SDR. If not, see <http://www.gnu.org/licenses/>.
#

set(OUTPUTFILTER_ADAPTER_SOURCES 
     file_output_filter.cc 
     null_sink_output_filter.cc 
)

include_directories(
     $(CMAKE_CURRENT_SOURCE_DIR)
     ${CMAKE_SOURCE_DIR}/src/core/interfaces
     ${CMAKE_SOURCE_DIR}/src/core/receiver
     ${GNURADIO_CORE_INCLUDE_DIRS}
     ${GNURADIO_GRUEL_INCLUDE_DIRS}
)

add_library(out_adapters ${OUTPUTFILTER_ADAPTER_SOURCES})