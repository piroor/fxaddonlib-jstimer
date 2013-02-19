# JavaScript Timer Library

## Usage

    var namespace = {};
    Components.utils.import('resource://foo-modules/jstimer.jsm', namespace);
    
    var callback = function(aMessage) { alert(aMessage); };
    var timeout = namespace.setTimeout(callback, 1000, 'OK');
    namespace.clearTimeout(timeout);
    var interval = namespace.setInterval(callback, 1000, 'OK');
    namespace.clearInterval(interval);

