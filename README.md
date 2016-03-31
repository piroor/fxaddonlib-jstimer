# JavaScript Timer Library

**important note**: this project is completely deprecated by [Timer.jsm](https://developer.mozilla.org/docs/Mozilla/JavaScript_code_modules/Timer.jsm). Use it instead of this.

## Usage

    var namespace = {};
    Components.utils.import('resource://foo-modules/jstimer.jsm', namespace);
    
    var callback = function(aMessage) { alert(aMessage); };
    var timeout = namespace.setTimeout(callback, 1000, 'OK');
    namespace.clearTimeout(timeout);
    var interval = namespace.setInterval(callback, 1000, 'OK');
    namespace.clearInterval(interval);

