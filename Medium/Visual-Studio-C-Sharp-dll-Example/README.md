# Visual-Studio-C#-dll-Example
### Front Panel
![Front Panel](https://github.com/Offliners/LabVIEW_projects/blob/master/Medium/Visual-Studio-C-Sharp-dll-Example/Visual-Studio-C-Sharp-dll-Example.vi%20Front%20Panel.png)

### Block Diagram
![Block Diagram](https://github.com/Offliners/LabVIEW_projects/blob/master/Medium/Visual-Studio-C-Sharp-dll-Example/Visual-Studio-C-Sharp-dll-Example.vi%20Block%20Diagram.png)

### C# Code
```Csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace MyTimerEvent
{
    public class MyTimer
    {
        private static int numCounts;

        public void nulnumCounts()
        {
            numCounts = 0;
        }

        public int GetNumCounts()
        {
            return numCounts;
        }

        public void IncNumCounts()
        {
            numCounts += 1;
        }

        private int _intervalMs;

        public int IntervalMs
        {
            get
            {
                return _intervalMs;
            }
            set
            {
                if (value > 0)
                    this._intervalMs = value;
                else
                    this._intervalMs = 1;
            }
        }
    }
}
```
