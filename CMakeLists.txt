# Copyright 2008, 2009, 2010, Olivier Stasse, JRL, CNRS/AIST
#
# This file is part of sample-humanoid-robot.
# sample-humanoid-robot is free software: you can redistribute it and/or modify
# it under the terms of the GNU Lesser General Public License as published by
# the Free Software Foundation, either version 3 of the License, or
# (at your option) any later version.
#
# sample-humanoid-robot is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Lesser Public License for more details.
# You should have received a copy of the GNU Lesser General Public License
# along with sample-humanoid-robot.  If not, see <http://www.gnu.org/licenses/>.

# Requires at least CMake 2.6 to configure the package.
CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

INCLUDE(cmake/base.cmake)
INCLUDE(cmake/cpack.cmake)

SET(PROJECT_NAME sample-humanoid-robot)
SET(PROJECT_VERSION 0.1.0)
SET(PROJECT_DESCRIPTION "sample-humanoid-robot")
SET(PROJECT_URL "http://github.com/jrl-umi3218/sample-humanoid-robot")


SETUP_PROJECT()
SETUP_PROJECT_CPACK()

SET(${PROJECT_NAME}_DATA 
  data/sample.wrl
  data/sampleInitConfig.dat
  data/sampleLinkJointRank.xml
  data/sampleSpecificities.xml
)

SETUP_PROJECT_FINALIZE()
