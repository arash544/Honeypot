<template>
  <header class="nav-img">
    <div class="nav-area">
      <div class="nav-wrapper">
        <a class="parent-logo" href>
          <img
            class="logo-image"
            src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4KPCEtLSBHZW5lcmF0b3I6IEFkb2JlIElsbHVzdHJhdG9yIDE4LjEuMSwgU1ZHIEV4cG9ydCBQbHVnLUluIC4gU1ZHIFZlcnNpb246IDYuMDAgQnVpbGQgMCkgIC0tPgo8c3ZnIHZlcnNpb249IjEuMSIgaWQ9IkxpdmVsbG9fMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB4bWxuczp4bGluaz0iaHR0cDovL3d3dy53My5vcmcvMTk5OS94bGluayIgeD0iMHB4IiB5PSIwcHgiCgkgdmlld0JveD0iMCAwIDQzMC43IDEwOC43IiBlbmFibGUtYmFja2dyb3VuZD0ibmV3IDAgMCA0MzAuNyAxMDguNyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI+CjxnPgoJPGc+CgkJPHBhdGggZmlsbD0iI0ZGQkUwRiIgZD0iTTg1LDYxLjZjLTAuNS02LjgtMi4xLTEzLjQtNC41LTE5LjVjLTAuNy0xLjYtMS40LTMuMi0yLjEtNC43YzIuOC0xLjYsNC43LTQuNyw0LjctOC4xCgkJCWMwLTUuMi00LjItOS41LTkuNS05LjVINjVoLTIuOEgyN2gtMi44aC04LjVjLTUuMiwwLTkuNSw0LjItOS41LDkuNWMwLDMuNSwxLjksNi41LDQuNiw4LjFjLTAuOCwxLjUtMS41LDMuMS0yLjEsNC43CgkJCWMtMi41LDYuMS00LjEsMTIuNi00LjYsMTkuNWMwLDAuOC0wLjEsMS42LTAuMSwyLjVjMCw1LjksMSwxMS42LDIuNywxNi45YzAuNSwxLjUsMS41LDQuMSwyLjgsNS44YzAuMSwwLjIsMC4zLDAuNCwwLjQsMC41CgkJCWMwLDAsMCwwLDAuMSwwLjFjMC41LDAuNywxLjIsMS40LDIsMi4xYzAuOCwwLjcsMS43LDEuNCwyLjgsMmMxLDAuNiwyLjMsMSwzLjUsMS4yYzEuMywwLjIsMi42LDAsMy42LTAuN2MxLTAuNywxLjgtMS45LDIuMi0zLjMKCQkJYzAuOS0yLjgsMC44LTYsMC41LTguOGMtMC4zLTIuOS0wLjgtNS42LTEuMy03LjhjLTEuMS00LjYtMi4xLTcuNS0yLjEtNy41czEuMiwyLjksMi42LDcuNGMwLjcsMi4zLDEuNCw0LjksMS45LDcuOAoJCQljMC41LDIuOSwwLjgsNi4xLDAuMSw5LjRjLTAuNCwxLjYtMS4yLDMuMy0yLjYsNC41Yy0xLjUsMS4yLTMuMywxLjUtNC45LDEuNmMtMS43LDAtMy4zLTAuNC00LjYtMC45Yy0wLjItMC4xLTAuMy0wLjEtMC41LTAuMgoJCQljMi41LDMuOCw1LjYsNy4zLDksMTAuNGMxLjgsMSw0LjgsMS43LDguNy0wLjNjNi44LTMuNSwxMy43LTMuOSwxMy43LTMuOXM2LjgsMC40LDEzLjcsMy45YzQuNiwyLjQsNy45LDEsOS41LTAuMgoJCQljMy4yLTIuOSw2LTYuMiw4LjQtOS44Yy0wLjIsMC4xLTAuMywwLjEtMC40LDAuMmMtMS40LDAuNS0yLjksMC45LTQuNiwwLjljLTEuNiwwLTMuNS0wLjQtNC45LTEuNmMtMS41LTEuMi0yLjMtMi45LTIuNi00LjUKCQkJYy0wLjctMy4zLTAuNC02LjUsMC4xLTkuNGMwLjUtMi45LDEuMi01LjYsMS45LTcuOGMxLjQtNC41LDIuNi03LjQsMi42LTcuNHMtMSwzLTIuMSw3LjVjLTAuNSwyLjMtMSw1LTEuMyw3LjgKCQkJYy0wLjMsMi45LTAuNCw2LDAuNSw4LjhjMC40LDEuNCwxLjIsMi42LDIuMiwzLjNjMSwwLjcsMi4zLDAuOSwzLjYsMC43YzEuMi0wLjIsMi40LTAuNiwzLjUtMS4yYzEuMS0wLjYsMi0xLjMsMi44LTIKCQkJYzEuMS0wLjksMS45LTEuOSwyLjUtMi43YzEtMS40LDEuOC0zLjMsMi40LTQuOGMyLTUuNiwzLTExLjYsMy0xNy45Qzg1LDYzLjMsODUsNjIuNCw4NSw2MS42eiIvPgoJCTxjaXJjbGUgZmlsbD0iI0ZGRkZGRiIgY3g9IjI3LjUiIGN5PSIzNi4xIiByPSI4LjYiLz4KCQk8cGF0aCBmaWxsPSIjMUYyMjI4IiBkPSJNMTUuNywyNC41Yy0yLjYsMC00LjcsMi4xLTQuNyw0LjdjMCwxLjcsMC45LDMuMiwyLjIsNGMxLjYtMi43LDMuNS01LjMsNS41LTcuNwoJCQlDMTcuOSwyNSwxNi45LDI0LjUsMTUuNywyNC41eiIvPgoJCTxwYXRoIGZpbGw9IiMxRjIyMjgiIGQ9Ik03My41LDI0LjVjLTEuMSwwLTIuMiwwLjQtMywxLjFjMiwyLjQsMy44LDUsNS41LDcuN2MxLjMtMC44LDIuMy0yLjMsMi4zLTQKCQkJQzc4LjIsMjYuNyw3Ni4xLDI0LjUsNzMuNSwyNC41eiIvPgoJCTxwYXRoIGZpbGw9IiMxRjIyMjgiIGQ9Ik0yNy41LDMyLjJjLTAuMywwLTAuNSwwLTAuOCwwLjFjMC4yLDAuMywwLjIsMC42LDAuMiwxYzAsMS4yLTAuOSwyLjEtMi4xLDIuMWMtMC40LDAtMC44LTAuMS0xLjEtMC4zCgkJCWMtMC4xLDAuMy0wLjEsMC42LTAuMSwxYzAsMi4xLDEuNywzLjgsMy44LDMuOGMyLjEsMCwzLjgtMS43LDMuOC0zLjhDMzEuMywzMy45LDI5LjYsMzIuMiwyNy41LDMyLjJ6Ii8+CgkJPGNpcmNsZSBmaWxsPSIjRkZGRkZGIiBjeD0iNjEuNyIgY3k9IjM2LjEiIHI9IjguNiIvPgoJCTxwYXRoIGZpbGw9IiMxRjIyMjgiIGQ9Ik02MS43LDMyLjJjLTAuMywwLTAuNSwwLTAuOCwwLjFjMC4yLDAuMywwLjIsMC42LDAuMiwxYzAsMS4yLTAuOSwyLjEtMi4xLDIuMWMtMC40LDAtMC44LTAuMS0xLjEtMC4zCgkJCWMtMC4xLDAuMy0wLjEsMC42LTAuMSwxYzAsMi4xLDEuNywzLjgsMy44LDMuOHMzLjgtMS43LDMuOC0zLjhDNjUuNiwzMy45LDYzLjgsMzIuMiw2MS43LDMyLjJ6Ii8+CgkJPGNpcmNsZSBmaWxsPSIjRkZGRkZGIiBjeD0iNDQuNSIgY3k9IjUyLjciIHI9IjExLjciLz4KCQk8cGF0aCBmaWxsPSIjMUYyMjI4IiBkPSJNNTAuNiw0Ni4zYzAtMC4yLDAtMC4zLTAuMS0wLjVjMC0wLjEsMC0wLjEsMC0wLjFoMGMtMC4xLTAuMS0wLjEtMC4zLTAuMi0wLjRsMCwwYzAsMC0wLjctMS40LTUuNy0xLjR2MAoJCQljMCwwLDAsMCwwLDBjMCwwLDAsMCwwLDB2MGMtMi45LDAtNC40LDAuNS01LjEsMC45Yy0wLjQsMC4yLTAuOCwwLjUtMC45LDAuOWgwYzAsMCwwLDAuMSwwLDAuMWMwLDAuMS0wLjEsMC4zLTAuMSwwLjQKCQkJYzAsMCwwLDAsMCwwYzAsMC43LDAuMiwyLDEuOSwzLjRjMS41LDEuMiwyLjcsMS43LDMuNCwxLjh2MTIuOWMwLjMsMCwwLjUsMCwwLjgsMGMwLjMsMCwwLjUsMCwwLjgsMFY1MS42CgkJCWMwLjctMC4yLDEuOS0wLjYsMy40LTEuOEM1MC4zLDQ4LjQsNTAuNiw0Ny4xLDUwLjYsNDYuM0M1MC42LDQ2LjMsNTAuNiw0Ni4zLDUwLjYsNDYuM3oiLz4KCQk8cGF0aCBmaWxsPSIjRkZCRTBGIiBkPSJNMjUuNiwxNy4zaDM3LjljLTQuNS0zLjEtOS45LTUuMi0xNS42LTUuN2wyLjMtNi4zYzAsMC0xLjUtMS4yLTUuNi0xLjJzLTUuNiwxLjItNS42LDEuMmwyLjMsNi4zCgkJCUMzNS40LDEyLjEsMzAuMSwxNC4yLDI1LjYsMTcuM3oiLz4KCQk8cGF0aCBmaWxsPSIjRkZGRkZGIiBkPSJNMTAuNSw4Mi45YzAsMC0wLjYtMC44LTEuMy0yLjJjLTAuNy0xLjQtMS40LTMuMy0xLjktNS4zYy0wLjUtMi0wLjctNC0wLjctNS42YzAtMS41LDAuMS0yLjYsMC4xLTIuNgoJCQlzMC4xLDAuMiwwLjIsMC43QzcsNjguNCw3LjEsNjksNy4zLDY5LjhjMC4zLDEuNSwwLjcsMy40LDEuMiw1LjRjMC40LDIsMC45LDMuOSwxLjMsNS4zYzAuMiwwLjcsMC40LDEuMywwLjUsMS44CgkJCUMxMC41LDgyLjcsMTAuNSw4Mi45LDEwLjUsODIuOXoiLz4KCQk8cGF0aCBmaWxsPSIjRkZGRkZGIiBkPSJNNjkuMSw3MC42YzAsMCwwLDAuNy0wLjEsMS43Yy0wLjEsMS0wLjMsMi4zLTAuNiwzLjZjLTAuMywxLjMtMC42LDIuNi0wLjksMy41Yy0wLjEsMC41LTAuMywwLjktMC40LDEuMgoJCQlDNjcsODAuOCw2Nyw4MSw2Nyw4MXMtMC4xLTAuNy0wLjEtMS43YzAtMSwwLjEtMi40LDAuNC0zLjdjMC4zLTEuMywwLjctMi42LDEuMS0zLjVDNjguNyw3MS4yLDY5LjEsNzAuNiw2OS4xLDcwLjZ6Ii8+CgkJPHBhdGggZmlsbD0iI0ZGRkZGRiIgZD0iTTE1LjYsMjFjMCwwLTAuNywwLjMtMS42LDAuOGMtMC41LDAuMy0xLDAuNi0xLjUsMWMtMC41LDAuNC0xLDAuOS0xLjUsMS40Yy0wLjUsMC41LTAuOSwxLjEtMS4zLDEuNgoJCQljLTAuNCwwLjYtMC43LDEuMS0wLjksMS42Yy0wLjMsMC41LTAuNSwwLjktMC42LDEuMmMtMC4xLDAuMy0wLjIsMC41LTAuMiwwLjVzMC0wLjIsMC0wLjVjMC0wLjMsMC0wLjgsMC4yLTEuNAoJCQljMC4xLTAuNiwwLjQtMS4yLDAuNy0xLjhjMC4zLTAuNiwwLjgtMS4zLDEuMy0xLjhjMS4xLTEuMSwyLjUtMS45LDMuNi0yLjJDMTQuOCwyMC45LDE1LjYsMjEsMTUuNiwyMXoiLz4KCTwvZz4KCTxnPgoJCTxwYXRoIGZpbGw9IiMxRjIyMjgiIGQ9Ik0xNzQuNSw0NS41Yy01LjQsMC0xMCwxLjctMTMuNyw1LjJjLTMuNywzLjUtNS42LDcuOS01LjYsMTMuM3MxLjksOS44LDUuNiwxMy4zYzMuNywzLjUsOC4zLDUuMiwxMy43LDUuMgoJCQljNS41LDAsMTAuMS0xLjcsMTMuOC01LjJjMy43LTMuNSw1LjYtNy45LDUuNi0xMy4zcy0xLjktOS44LTUuNi0xMy4zQzE4NC41LDQ3LjIsMTc5LjksNDUuNSwxNzQuNSw0NS41eiBNMTgyLDcxLjkKCQkJYy0yLDIuMS00LjUsMy4xLTcuNSwzLjFjLTIuOSwwLTUuNC0xLTcuNC0zLjFjLTItMi0zLTQuNy0zLTcuOWMwLTMuMiwxLTUuOCwzLTcuOWMyLTIuMSw0LjUtMy4xLDcuNC0zLjFjMi45LDAsNS40LDEsNy40LDMuMQoJCQljMi4xLDIuMSwzLjEsNC43LDMuMSw3LjlDMTg1LDY3LjIsMTg0LDY5LjgsMTgyLDcxLjl6Ii8+CgkJPHBhdGggZmlsbD0iIzFGMjIyOCIgZD0iTTI2MC43LDQ1LjVjLTUuMywwLTkuNiwxLjctMTIuOSw1LjJjLTMuMywzLjQtNSw3LjktNSwxMy4zYzAsNS4yLDEuNyw5LjUsNS4yLDEzLjEKCQkJYzMuNSwzLjYsOC4xLDUuNCwxMy43LDUuNGMxLjcsMCwzLjMtMC4yLDQuOS0wLjZjMS42LTAuNCwyLjktMC44LDMuOS0xLjNjMS0wLjUsMi0xLDIuOS0xLjZjMC45LTAuNiwxLjYtMSwxLjgtMS4zCgkJCWMwLjMtMC4zLDAuNS0wLjUsMC42LTAuNmwtMy43LTYuMWwtMS4yLDFjLTAuOCwwLjYtMiwxLjMtMy43LDJjLTEuNywwLjctMy4zLDEtNSwxYy0yLjgsMC01LjEtMC44LTcuMS0yLjVjLTItMS43LTMuMS00LTMuNS03CgkJCWgyNC40bDAuMi0zLjNjMC00LjgtMS40LTguOC00LjItMTJDMjY5LjQsNDcuMSwyNjUuNiw0NS41LDI2MC43LDQ1LjV6IE0yNTIuMSw1OS40YzAuNS0yLjIsMS41LTQsMy01LjJjMS41LTEuMywzLjQtMS45LDUuNi0xLjkKCQkJYzEuOCwwLDMuNCwwLjcsNC43LDJjMS4zLDEuMywxLjksMywyLDUuMUgyNTIuMXoiLz4KCQk8cGF0aCBmaWxsPSIjMUYyMjI4IiBkPSJNMzQyLjQsNDUuNWMtMS41LDAtMywwLjItNC4zLDAuNmMtMS40LDAuNC0yLjQsMC45LTMuMiwxLjNjLTAuOCwwLjUtMS41LDEuMS0yLjEsMS43CgkJCWMtMC42LDAuNi0xLjEsMS4xLTEuMiwxLjNjLTAuMiwwLjMtMC4zLDAuNS0wLjQsMC42aC0wLjF2LTEuNGMwLTIuMy0xLjUtMy40LTQuNC0zLjRoLTIuMmgtNS42aC04LjJjLTIuNCwwLTQsMS4xLTQuNywzLjMKCQkJbC0wLjIsMC42bC03LDIwLjNsLTguMy0yMC45Yy0wLjUtMS4yLTEtMi4xLTEuNy0yLjZjLTAuNy0wLjUtMS43LTAuOC0yLjktMC44aC0yLjZIMjgwaC0xbDEsMi4ybDIuOSw2LjVsMTEuOCwyNi41bC0xLjIsMi43CgkJCWMtMS4yLDMtMy4yLDQuNS01LjgsNC41Yy0xLjksMC0zLjYtMC44LTUuMS0yLjRsLTMuNCw2LjJsMSwwLjljMC42LDAuNiwxLjcsMS4yLDMuMiwxLjhjMS41LDAuNiwzLDAuOSw0LjcsMC45CgkJCWMyLjgsMCw1LjMtMC44LDcuNS0yLjNjMi4zLTEuNSw0LTMuOCw1LjItNi45TDMxMy41LDU1YzAuMy0wLjgsMS0xLjIsMi0xLjJoMy4zaDEuMWgxLjdjMSwwLDEuNSwwLjUsMS41LDEuNXY0MC4xaDguN1Y4MC44CgkJCWMwLTEuMiwwLTIuMi0wLjEtM2gwLjFsMSwxLjJjMC42LDAuNywxLjgsMS41LDMuNSwyLjNjMS43LDAuOCwzLjYsMS4yLDUuNiwxLjJjNC43LDAsOC42LTEuNywxMS42LTUuMWMzLTMuNCw0LjYtNy45LDQuNi0xMy40CgkJCWMwLTUuNS0xLjQtOS45LTQuMy0xMy40QzM1MSw0Ny4yLDM0Ny4yLDQ1LjUsMzQyLjQsNDUuNXogTTM0Ni43LDcyLjFjLTEuNywyLTMuOCwyLjktNi40LDIuOWMtMi44LDAtNC45LTEuMS02LjQtMy4yCgkJCWMtMS41LTIuMS0yLjMtNC43LTIuMy03LjZjMC0zLjcsMC45LTYuNSwyLjYtOC4zYzEuNy0xLjksMy44LTIuOCw2LjMtMi44YzIuNiwwLDQuNywxLDYuNCwzYzEuNiwyLDIuNCw0LjcsMi40LDgKCQkJQzM0OS4zLDY3LjUsMzQ4LjQsNzAuMSwzNDYuNyw3Mi4xeiIvPgoJCTxwYXRoIGZpbGw9IiMxRjIyMjgiIGQ9Ik0zODEuOSw0NS41Yy01LjQsMC0xMCwxLjctMTMuNyw1LjJjLTMuNywzLjUtNS42LDcuOS01LjYsMTMuM3MxLjksOS44LDUuNiwxMy4zYzMuNywzLjUsOC4zLDUuMiwxMy43LDUuMgoJCQljNS41LDAsMTAuMS0xLjcsMTMuOC01LjJjMy43LTMuNSw1LjYtNy45LDUuNi0xMy4zcy0xLjktOS44LTUuNi0xMy4zQzM5MS45LDQ3LjIsMzg3LjMsNDUuNSwzODEuOSw0NS41eiBNMzg5LjQsNzEuOQoJCQljLTIsMi4xLTQuNSwzLjEtNy41LDMuMWMtMi45LDAtNS40LTEtNy40LTMuMWMtMi0yLTMtNC43LTMtNy45YzAtMy4yLDEtNS44LDMtNy45YzItMi4xLDQuNS0zLjEsNy40LTMuMWMyLjksMCw1LjQsMSw3LjQsMy4xCgkJCWMyLjEsMi4xLDMuMSw0LjcsMy4xLDcuOUMzOTIuNCw2Ny4yLDM5MS40LDY5LjgsMzg5LjQsNzEuOXoiLz4KCQk8cGF0aCBmaWxsPSIjMUYyMjI4IiBkPSJNNDI1LjEsNzQuMmMtMS44LDAtMy40LTAuNS00LjgtMS40Yy0xLjUtMC45LTIuMi0yLjctMi4yLTUuMlY1My4zaDh2LTdoLTh2LTkuNmgtOC42djkuNmgtNC44djdoNC42djE1LjQKCQkJYzAsMi4zLDAuNCw0LjIsMS4xLDUuOWMwLjcsMS43LDEuNiwzLDIuNiwzLjljMSwwLjksMi4zLDEuNiwzLjcsMi4yYzEuNCwwLjYsMi43LDAuOSwzLjgsMS4xYzEuMSwwLjIsMi4zLDAuMiwzLjUsMC4yCgkJCWMxLjEsMCwyLTAuMSwyLjctMC4ydi03LjdMNDI1LjEsNzQuMnoiLz4KCQk8cGF0aCBmaWxsPSIjMUYyMjI4IiBkPSJNMTM5LjMsMzcuMnYxNi4xaC0yMS43VjM3LjJjMC0xLjYtMC40LTIuOC0xLjEtMy42Yy0wLjctMC44LTEuOS0xLjEtMy42LTEuMWgtNC40djkuMnYxNHYyNS45aDkuMVY2MQoJCQloMjEuN3YyMC42aDkuMVY2MS4zVjQxLjd2LTkuMkgxNDRDMTQwLjksMzIuNSwxMzkuMywzNCwxMzkuMywzNy4yeiIvPgoJCTxwYXRoIGZpbGw9IiMxRjIyMjgiIGQ9Ik0yMjIuNyw0NS41Yy0zLjIsMC01LjgsMC43LTcuOSwyLjJjLTIuMSwxLjUtMy42LDMuMi00LjYsNS4xaC0wLjFsMC4xLTEuNXYtMWMwLTIuNi0xLjUtMy45LTQuNi0zLjloLTMuOAoJCQl2OXYxMy4ydjEzaDguN1Y2NS40YzAtMS44LDAuMi0zLjMsMC43LTQuN2MwLjYtMi4yLDEuOC0zLjksMy41LTUuMmMxLjctMS4zLDMuNy0yLDYtMmMyLjEsMCwzLjUsMC42LDQuMywxLjgKCQkJYzAuOCwxLjIsMS4yLDMsMS4yLDUuNHYxNi4yYzAsMS43LDAuNCwyLjksMS4xLDMuNmMwLjcsMC43LDEuOSwxLjEsMy42LDEuMWg0LjF2LTguOXYtNS42di04LjJDMjM1LjEsNTAsMjMwLjksNDUuNSwyMjIuNyw0NS41eiIKCQkJLz4KCTwvZz4KPC9nPgo8L3N2Zz4K"
            alt
          />
        </a>

        <nav>
          <button @click="showMenu" class="menu-icon">
            <svg
              id="Layer_1"
              enable-background="new 0 0 512 512"
              height="20"
              viewBox="0 0 512 512"
              width="20"
              xmlns="http://www.w3.org/2000/svg"
              fill="gray"
            >
              <path
                d="m464.883 64.267h-417.766c-25.98 0-47.117 21.136-47.117 47.149 0 25.98 21.137 47.117 47.117 47.117h417.766c25.98 0 47.117-21.137 47.117-47.117 0-26.013-21.137-47.149-47.117-47.149z"
              />
              <path
                d="m464.883 208.867h-417.766c-25.98 0-47.117 21.136-47.117 47.149 0 25.98 21.137 47.117 47.117 47.117h417.766c25.98 0 47.117-21.137 47.117-47.117 0-26.013-21.137-47.149-47.117-47.149z"
              />
              <path
                d="m464.883 353.467h-417.766c-25.98 0-47.117 21.137-47.117 47.149 0 25.98 21.137 47.117 47.117 47.117h417.766c25.98 0 47.117-21.137 47.117-47.117 0-26.012-21.137-47.149-47.117-47.149z"
              />
            </svg>
          </button>
          <ul ref="menu">
            <li>
              <a class="nav-link" href="/">For Talents</a>
            </li>
            <li>
              <a class="nav-link" href="/">For Employers</a>
            </li>
            <li>
              <a class="nav-link" href="/">
                <img
                  class="navbar-img"
                  src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxMDYuMDQgMTA2LjA0Ij48ZGVmcz48c3R5bGU+LmNscy0xe2ZpbGw6I2ZmZjt9PC9zdHlsZT48L2RlZnM+PGcgaWQ9IkxheWVyXzIiIGRhdGEtbmFtZT0iTGF5ZXIgMiI+PGcgaWQ9IkxheWVyXzEtMiIgZGF0YS1uYW1lPSJMYXllciAxIj48Y2lyY2xlIGN4PSI1My4wMiIgY3k9IjUzLjAyIiByPSI1My4wMiIvPjxwYXRoIGNsYXNzPSJjbHMtMSIgZD0iTTE2LjE2LDYxLjM1di0uNzNjMC0xLjY3LDEtMi45MSwzLjIxLTIuOTFzMy4yLDEuMjQsMy4yLDIuOTF2LjczYzAsMS42OC0xLDIuOTEtMy4yLDIuOTFTMTYuMTYsNjMsMTYuMTYsNjEuMzVaIi8+PHBhdGggY2xhc3M9ImNscy0xIiBkPSJNMjUuODIsNTQuMjljMC02LjEyLDMuMTctMTAsOC45Mi0xMCwzLjg2LDAsNi41MiwxLjg2LDcuNjUsNUwzOCw1MS4xOWEzLjE4LDMuMTgsMCwwLDAtMy4yOC0yLjYyYy0yLjE5LDAtMy4zMiwxLjU3LTMuMzIsNHYzLjU3YzAsMi40LDEuMTMsMy45MywzLjMyLDMuOTNzMy0xLjMxLDMuNTctMi44NEw0Mi40OSw1OWMtMS4yNywzLjY0LTQsNS4yOC03Ljc1LDUuMjhDMjksNjQuMywyNS44Miw2MC40LDI1LjgyLDU0LjI5WiIvPjxwYXRoIGNsYXNzPSJjbHMtMSIgZD0iTTU3LDYwLjY2aC0uMThhNS4xOSw1LjE5LDAsMCwxLTUuMzYsMy42NGMtMy44OSwwLTYtMi43My02LTcuNTR2LTEyaDUuMzlWNTYuMjljMCwyLjMzLjc3LDMuNjQsMi43MywzLjY0LDEuNjgsMCwzLjM5LTEsMy4zOS0yLjc3VjQ0Ljc1aDUuMzlWNjMuODZINTdaIi8+PHBhdGggY2xhc3M9ImNscy0xIiBkPSJNNzIuNDgsNjMuODZjLTMuNjgsMC01LjM1LTEuODUtNS4zNS01LjI0VjM2LjkyaDUuMzlWNTkuNjhoMi40djQuMThaIi8+PHBhdGggY2xhc3M9ImNscy0xIiBkPSJNODQuNDUsNjMuODZjLTMuNzEsMC01LjY4LTEuOTMtNS42OC01LjU3VjQ4LjkzSDc2LjA4VjQ0Ljc1aDEuMzRjMS40NiwwLDEuOS0uNzMsMS45LTJWMzkuNThoNC44NHY1LjE3SDg4djQuMThIODQuMTZWNTkuNjhoMy41djQuMThaIi8+PC9nPjwvZz48L3N2Zz4="
                  alt
                />Dev Community
              </a>
            </li>
            <li>
              <a class="nav-link" href="/">About Us</a>
            </li>
            <li>
              <a class="nav-link" href="/">Login</a>
            </li>
            <li>
              <a class="btn btn-primary btn-signup nav-link" href="/">Sign up</a>
            </li>
          </ul>
        </nav>
        <ul class="language">
          <li class="lang-li">
            <a class="lang-link" href="/">EN</a>
          </li>
          <li class="lang-li">
            <a class="lang-link" href="/">DE</a>
          </li>
          <li class="lang-li">
            <a class="lang-link" href="/">NL</a>
          </li>
        </ul>
      </div>
      <div class="wrapper">
        <h1>
          Choose a
          <br />
          <b>Job You Love</b>
        </h1>
        <p>Honeypot is Europe’s developer-focused job platform. Create a profile and let companies apply to you.</p>
        <div class="btn-wrapper">
          <a class="btn-job" href="/">Find Me a Job!</a>
          <a class="btn-hire" href="/">I'm Hiring</a>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "Navbar",
  methods: {
    showMenu() {
      this.$refs["menu"].classList.toggle("menu-block");
    }
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  display: flex;
  margin-top: 100px;
  margin-left: 330px;
  flex-direction: column;
  width: 380px;
  padding: 10px;
  @media only screen and (max-width: 768px) {
    width: 100%;
    margin-top: 300px;
    margin-left: 0px;
  }
  @media only screen and (max-width: 420px) {
    margin-top: 200px;
  }
}
.btn-wrapper {
  flex-direction: row;
  width: 100%;
  margin-top: 10px;
}
p {
  color: gray;
  margin-top: 10px;
  line-height: 1.3;
  font-weight: 500;
  font-size: 20px;
  @media only screen and (max-width: 768px) {
    padding-right: 140px;
  }
}
.btn-job {
  color: #cea000;
  border: 1px solid #fff2c6;
  background-color: #fff2c6;
  padding: 3px 10px;
  border-radius: 4px;
}
.btn-hire {
  margin-left: 50px;
  color: gray;
  text-decoration: underline;
}
.nav-img {
  background: url("https://www.honeypot.io/static/index.header.svg") no-repeat
    100% 0;
  background-size: contain;
  position: relative;
  height: 600px;
}
.nav-area {
  position: relative;
  height: 70px;
  top: 0;
  left: 0;
  right: 0;
  width: 100%;
}
.parent-logo {
  width: 30%;
  justify-content: flex-end;
  display: flex;
  margin-top: 10px;
  @media only screen and (max-width: 768px) {
    position: absolute;
    justify-content: center;
    margin-top: 20px;
    left: 35%;
    @media only screen and (max-width: 420px) {
      left: 30%;
    }
  }
}
.logo-image {
  height: 35px;
  text-align: center;
  @media only screen and (max-width: 768px) {
    justify-content: center;
    display: flex;
  }
}
.nav-wrapper {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-direction: row;
}
nav {
  display: flex;
  width: 60%;
  position: relative;

  margin-top: 20px;
  @media only screen and (max-width: 768px) {
    order: -1;
  }
}
ul {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  width: 100%;
  @media only screen and (max-width: 768px) {
    position: absolute;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    top: 0px;
    bottom: 0;
    left: -100%;
    right: 0;
    background-color: white;
    cursor: pointer;

    &.menu-block {
      left: -120px;
      top: 50px;
    }
  }
  @media only screen and (max-width: 420px) {
    &.menu-block {
      left: -55px;
      top: 50px;
    }
  }
}
.navbar-img {
  height: 20px;
}
li {
  list-style-type: none;
  font-weight: 600;
}
.nav-link {
  color: gray;
}
.btn-signup {
  color: white;
}
.language {
  width: 30%;
  display: flex;
  justify-content: flex-start;
  margin-top: 20px;
  @media only screen and (max-width: 768px) {
    padding-left: 0;
    justify-content: center;
    left: 70%;
    right: 0;
    flex-direction: row;
    justify-content: center;
    position: absolute;
    margin-top: 50px;
    @media only screen and (max-width: 420px) {
      margin-top: 55px;
      left: 67%;
    }
  }
}
.lang-li {
  justify-content: flex-end;
}
.lang-link {
  margin: 0px 5px;
  color: gray;
  @media only screen and (max-width: 420px) {
  }
}
.menu-icon {
  background-color: transparent;
  border-radius: 10px;
  font-size: 14px;
  margin-left: 100px;
  outline: none;
  border: none;
  margin-top: 20px;
  cursor: pointer;
  display: none;
  outline: none;
  @media only screen and (max-width: 768px) {
    display: block;
    z-index: 1000;
    position: relative;
    outline: none;
    &:active,
    &:hover,
    &:focus {
      outline: none;
    }
  }
  @media only screen and (max-width: 420px) {
    margin-left: 50px;
  }
}
</style>