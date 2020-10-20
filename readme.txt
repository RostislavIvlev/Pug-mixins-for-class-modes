mixin name(options)

  -
    var mods = '';
    if (typeof(options) !== 'undefined' && options.mod) {
        var modList = options.mod.splt(',');
        for (var i = 0; i < modList.length; i++) {
            mods = mods + ' className_' + modList[i].trim();
        }
    }

  .className(class= mods)