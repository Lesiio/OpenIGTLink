PROJECT(Klient)

cmake_minimum_required(VERSION 2.4)
if(COMMAND cmake_policy)
  cmake_policy(SET CMP0003 NEW)
endif(COMMAND cmake_policy)

find_package(OpenIGTLink REQUIRED)

include(${OpenIGTLink_USE_FILE})

ADD_EXECUTABLE(NowyKlient   NowyKlient.cxx)
TARGET_LINK_LIBRARIES(NowyKlient OpenIGTLink)

#ADD_EXECUTABLE(PointServerK   PointServerK.cxx)
#TARGET_LINK_LIBRARIES(PointServerK OpenIGTLink)

#ADD_EXECUTABLE(PointListServerK   PointListServerK.cxx)
#TARGET_LINK_LIBRARIES(PointListServerK OpenIGTLink)

#ADD_EXECUTABLE(PointClient3K   PointClient3K.cxx)
#TARGET_LINK_LIBRARIES(PointClient3K OpenIGTLink)

#ADD_EXECUTABLE(PointServer3K   PointServer3K.cxx)
#TARGET_LINK_LIBRARIES(PointServer3K OpenIGTLink)


PROJECT(Serwer)


find_package(OpenIGTLink REQUIRED)


include(${OpenIGTLink_USE_FILE})



ADD_EXECUTABLE(NowySerwer  NowySerwer.cxx)

TARGET_LINK_LIBRARIES(NowySerwer OpenIGTLink)


#ADD_EXECUTABLE(ReceiveClientS  ReceiveClientS.cxx)

#TARGET_LINK_LIBRARIES(ReceiveClientS OpenIGTLink)
