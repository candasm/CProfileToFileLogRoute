CProfileToFileLogRoute
======================

CProfileToFileLogRoute

This component for write yii profiling messages to file.

CProfileToFileLogRoute.php add in import list under config.file
Log component settings:
<code>
        'log' => array(
            'class' => 'CLogRouter',
            'routes' => array(
                array(
                    'class' => 'CProfileToFileLogRoute',
                    'logFile' => 'profiling.log',
                ),
            ),
        ),
</code>
Useing(Same as profiling): 
<code>
    Yii::beginProfile('sleep');
    sleep(1);
    Yii::endProfile('sleep);
</code>