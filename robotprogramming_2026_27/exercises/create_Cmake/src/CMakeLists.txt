add_library(core_library SHARED
messages/base_sensor_message.cpp
messages/pose_message.cpp
messages/odometry_message.cpp
utils/id_context.cpp
utils/deserializer.cpp
utils/property_identifiable.cpp
utils/serializer.cpp
utils/id_placeholder.cpp
utils/identifiable.cpp
utils/blob.cpp
utils/serializable.cpp
utils/object_data.cpp
utils/property_eigen.cpp
utils/serialization_context.cpp
utils/property_container_manager.cpp
utils/property_container.cpp
utils/property.cpp


    # TODO add other .cpp files
)

# TODO: Include the current directory ( . ) to the list of directories to search for header files
target_include_directories(core_library PUBLIC . ${EIGEN3_INCLUDE_DIR})

# TODO: Include the Eigen3 library to the list of libraries to link against
