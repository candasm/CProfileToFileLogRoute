CProfileToFileLogRoute
======================

CProfileToFileLogRoute

This component for write yii profiling messages to file.

CProfileToFileLogRoute.php add in import list under config.file
Log component settings:
<code><pre>
        'log' => array(
            'class' => 'CLogRouter',
            'routes' => array(
                array(
                    'class' => 'CProfileToFileLogRoute',
                    'logFile' => 'profiling.log',
                ),
            ),
        ),</pre>
</code>
Useing(Same as profiling): 
<code><pre>
    Yii::beginProfile('sleep');
    sleep(1);
    Yii::endProfile('sleep);
</pre>
</code>