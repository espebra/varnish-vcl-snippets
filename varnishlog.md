# Varnishlog for Varnish 4 cheat sheet

Group log records by request relationship, so that the response and any ESI includes are showed in human readable order:

    # varnishlog -g request

Show the responses that are slower than 2 seconds and their requests:

    # varnishlog -g request -q 'Timestamp:Resp[3] > 2.0'

Show the the ``5XX`` responses and their requests:

    # varnishlog -g request -q 'RespStatus >= 500'

Show old log entries from using the ``-d`` parameter:

    # varnishlog -g request -d -q 'RespStatus >= 500'

Filter away client requests that contain the request header ``foo``:

    # varnishlog -g request -q "not ReqHeader:foo"

Filter away backend responses that contain the response header ``bar``:

    # varnishlog -g request -q "not BerespHeader:bar"

Filter on URL, response status and method:

    # varnishlog -g request -q "ReqUrl ~ '/some/path' and RespStatus == 200 and ReqMethod ~ 'GET'"
