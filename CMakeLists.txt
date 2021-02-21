set(
  srcs
  src/tftp_ota_server.cpp
  src/tftp_server.cpp
  src/tftp_server_priv.h
  )

idf_component_register(
  .
  SRCS ${srcs}
  INCLUDE_DIRS "include"
  REQUIRES nvs_flash app_update
  )
