# develop_configuration_files

Develop the API data source for the software.

## TimeTableAuto 法定节假日

- 文件：`cn_public_holidays.json`
- Raw 地址（仓库需为 **Public** 时可用）：
  `https://raw.githubusercontent.com/cst-github/develop_configuration_files/main/cn_public_holidays.json`

字段说明：

- `holidays`：放假不填区间，`start` / `end` 为 `YYYY-MM-DD`，`name` 为节日名称
- `makeup_workdays`：调休上班日列表（即使周末也会填写）

每年国务院通知发布后，更新本文件并推送到 `main` 即可；客户端通过菜单「配置 → 更新法定节假日」拉取，无需重打包 exe。
