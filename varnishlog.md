# Varnishlog for Varnish 4 cheat sheet

Group log records by request relationship, so that the response and any ESI includes are showed in human readable order:

::
    varnishlog -g request

Show the responses that are slower than 2 seconds and their requests:

::
    varnishlog -g request -q 'Timestamp:Resp[3] > 2.0'

Show the the ``5XX`` responses and their requests:

::
    varnishlog -g request -q 'RespStatus >= 500'

