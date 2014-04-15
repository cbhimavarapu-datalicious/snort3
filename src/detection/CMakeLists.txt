
set (DETECTION_INCLUDES
    detection_defines.h
    rule_option_types.h
    rules.h
    signature.h
    treenodes.h
)

add_library (detection STATIC
    ${DETECTION_INCLUDES}
    detect.cc 
    detect.h 
    detection_options.cc
    detection_options.h
    detection_util.cc 
    detection_util.h 
    fpcreate.cc 
    fpcreate.h 
    fpdetect.cc 
    fpdetect.h 
    generators.h 
    pcrm.cc 
    pcrm.h 
    sfrim.cc 
    sfrim.h 
    signature.cc 
    treenodes.cc
    tag.cc 
    tag.h 
)

install(FILES ${DETECTION_INCLUDES}
    DESTINATION "${CMAKE_PROJECT_NAME}/detection"
)