# Generated from wayland-eglstream-controller.pro.

#####################################################################
## QWaylandEglStreamBufferIntegrationPlugin Plugin:
#####################################################################

qt_internal_add_plugin(QWaylandEglStreamBufferIntegrationPlugin
    OUTPUT_NAME qt-wayland-compositor-wayland-eglstream-controller
    TYPE wayland-graphics-integration-server
    SOURCES
        ../../../../hardwareintegration/compositor/wayland-eglstream-controller/waylandeglstreamcontroller.cpp ../../../../hardwareintegration/compositor/wayland-eglstream-controller/waylandeglstreamcontroller.h
        ../../../../hardwareintegration/compositor/wayland-eglstream-controller/waylandeglstreamintegration.cpp ../../../../hardwareintegration/compositor/wayland-eglstream-controller/waylandeglstreamintegration.h
        main.cpp
    INCLUDE_DIRECTORIES
        ../../../../hardwareintegration/compositor/wayland-eglstream-controller
    LIBRARIES
        EGL::EGL
        Wayland::Egl
        Wayland::Server
    PUBLIC_LIBRARIES
        Qt::CorePrivate
        Qt::EglSupportPrivate
        Qt::GuiPrivate
        Qt::WaylandCompositor
        Qt::WaylandCompositorPrivate
)

qt6_generate_wayland_protocol_server_sources(QWaylandEglStreamBufferIntegrationPlugin
    FILES
        ${CMAKE_CURRENT_SOURCE_DIR}/../../../../hardwareintegration/compositor/wayland-eglstream-controller/../../../3rdparty/protocol/wl-eglstream-controller.xml
)

#### Keys ignored in scope 1:.:.:wayland-eglstream-controller.pro:<TRUE>:
# OTHER_FILES = "wayland-eglstream-controller.json"
