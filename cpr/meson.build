sources = files(
	'auth.cpp',
    	'bearer.cpp',
    	'cookies.cpp',
    	'cprtypes.cpp',
    	'curl_container.cpp',
    	'curlholder.cpp',
    	'error.cpp',
    	'multipart.cpp',
    	'parameters.cpp',
    	'payload.cpp',
    	'proxies.cpp',
    	'proxyauth.cpp',
    	'session.cpp',
    	'timeout.cpp',
    	'unix_socket.cpp',
    	'util.cpp',
    	'response.cpp',
    	'redirect.cpp',
)

cpr = library(
	'cpr',
	sources: sources,
	dependencies: [libcurl],
	install: true,
	install_dir: [true],
	include_directories: incdir
)

cpr_dep = declare_dependency(include_directories: incdir, link_with: cpr)
