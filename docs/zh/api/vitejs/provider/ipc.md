# ipc 

## Constructor

- **Constructor params**: 

  * `path : string` 连接path  default: ''
  * `timeout : number` 超时时间（ms） default: 60000
  * `Object` 
	- `delimiter : string` : 分割符 default: `\n`
    - `retryTimes : number`: 重连超时时间
    - `retryInterval : number`: 重连间隔时长

- **Example**:

```javascript

import ipcProvider from "@vite/vitejs/dist/es5/provider/IPC";
const myIpc = new ipcProvider("~/.gvite/testdata/gvite.ipc");

```

## ipc provider

### 实例属性

|  名称  | 类型 | 说明 |
|:------------:|:-----:|:-----:|
| path | string | 连接路径 |
| delimiter | string | 分割符 |

### 实例方法
除provider实例的共有方法外

* `reconnect()`: 重连
* `disconnect()`: 取消连接
