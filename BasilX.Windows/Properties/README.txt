The items in this directory are created by pre-build actions
in BasilX.csproj. In particular, the actions are:

    echo %date% %time% > "$(ProjectDir)\Resources\BuildDate.txt"
    git rev-parse HEAD > "$(ProjectDir)\Resources\GitCommit.txt"

The files so created are set as embedded resources in BasilTest.csproj
and, as resources, their contents are available for the
BasilTest application.
