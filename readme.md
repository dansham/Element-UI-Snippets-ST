### Install

#### Manual Install
Copy the folder element-ui-snippets to the path directly:

+ **Mac**: /Users/*< your-user-name >*/Library/Application Support/Sublime Text 3/Packages/User/
+ **Windows**: *< your-installed-driver >* :\Users\ *< your-user-name >* \AppData\Roaming\Sublime Text 3\Packages\User\

#### Through Package Control

1. Install Package Control
2. Open Command Palette
3. Type: Package Control: Install Package, and hit Enter
4. Type: Element UI Snippets, and hit Enter

### Special Instruction：

1. For the components like `el-table` which need children components to be content, use `v-for` to loop to generate the children components.
2. By default, there would be no auto-complete hints in .html file or the template part in .vue file. If you want it to be shown, you should change the sublime text settings by yourself. Here are the steps (Mac version for example):
    1. Select menu: Sublime Text -> Preferences -> Settings
    2. Make sure the value of the option `auto_complete` is `true`
    3. In Preferences.sublime-settings--Users file, add this key-value:
        ````
        "auto_complete_triggers": [
            {
                "selector": "text.html",
                "characters": "l"
            }
        ],
        ````
    **Warning: this setting would trigger all sinppets which contain letter 'l' even they are not defined in Element UI Snippets.**

### Snippets List

1. All the Element UI tags below, ignore the closure and more detailed information. Such as `elr` to `<el-radio>`, actually that represents `<el-radio v-model="${1}" label="${2}">$3</el-radio>`
2. The sinppets' order follows the order of the components of Guide on Element UI official website basically. Supply extra General and Options parts.
3. Totally 104 snippets. 9 of them are not implemented yet.
4. **Only work in .html or .vue file.**



#### Basic Part
|No.|Trigger&nbsp;Key|Element Tag|
|:------:|:--------------:|:--------|
|1. | `elrow` | `<el-row>` |
|2. | `elcol` | `<el-col>` |
|3. | `elcon` | `<el-container>` |
|4. | `elas` | `<el-aside>` |
|5. | `elhe` | `<el-header>` |
|6. | `elma` | `<el-main>` |
|7. | `elfo` | `<el-footer>` |
|8. | `elcb` | `#409EFF` |
|9. | `elcs` | `#67C23A` |
|10. | `elcw` | `#E6A23C` |
|11. | `elcd` | `#F56C6C` |
|12. | `elci` | `#909399` |
|13. | TBD | `#303133` |
|14. | TBD | `#606266` |
|15. | TBD | `#909399` |
|16. | TBD | `#C0C4CC` |
|17. | TBD | `#DCDFE6` |
|18. | TBD | `#E4E7ED` |
|19. | TBD | `#EBEEF5` |
|20. | TBD | `#F2F6FC` |
|21. | `eltypo` | `font-family: "Helvetica Neue",Helvetica,"PingFang SC","Hiragino Sans GB","Microsoft YaHei","微软雅黑",Arial,sans-serif;` |
|22. | `elb` | `el-button` |

#### Form Part

No. |  Trigger Key | Element Tag
|:------:|:--------------:|:--------|
|1. | `elr` | `<el-radio>` |
|2. | `elrg` | `<el-radio-group>` |
|3. | `elc` | `<el-checkbox>` |
|4. | `elcg` | `<el-checkbox-group>` |
|5. | `eli` | `<el-input>` |
|6. | `elit` | `<el-input type="textarea">` |
|7. | `elin` | `<el-input-number>` |
|8. | `elsel` | `<el-select>` |
|9. | `elop` | `<el-option>` |
|10. | `elca` | `<el-cascader>` |
|11. | `elsw` | `<el-swtich>` |
|12. | `elsl` | `<el-slider>` |
|13. | `eltp` | `<el-time-picker>` |
|14. | `elts` | `<el-time-select>` |
|15. | `eldp` | `<el-date-picker>` |
|16. | `eldtp` | `<el-date-picker type="datetime">` |
|17. | `elu` | `<el-upload>` |
|18. | `elra` | `<el-rate>` |
|19. | `elcp` | `<el-color-picker>` |
|20. | `eltr` | `<el-transfer>` |
|21. | `elf` | `<el-form>` |
|22. | `elfi` | `<el-form-item>` |

#### Data Part

No. |  Trigger Key | Element Tag
|:------:|:--------------:|:--------|
|1. | `elta` | `<el-table>` |
|2. | `eltac` | `<el-table-column>` |
|3. | `eltag` | `<el-tag>` |
|4. | `eltags` | `<el-tag type="success">` |
|5. | `eltagi` | `<el-tag type="info">` |
|6. | `eltagw` | `<el-tag type="warning">` |
|7. | `eltagd` | `<el-tag type="danger">` |
|8. | `elpr` | `<el-progress>` |
|9. | `elprc` | `<el-progress type="circle">` |
|10. | `eltree` | `<el-tree>` |
|11. | `elpa` | `<el-pagination>` |
|12. | `elba` | `<el-badge>` |


#### Notice Part

No. |  Trigger Key | Element Tag
|:------:|:--------------:|:--------|
|1. | `elal` | `<el-alert>` |
|2. | `elals` | `<el-alert type="success">` |
|3. | `elali` | `<el-alert type="info">` |
|4. | `elalw` | `<el-alert type="warning">` |
|5. | `elale` | `<el-alert type="error">` |
|6. | `elloads` | 	`element-loading-*` |
|7. | `elme` | `this.$message({})` |
|8. | `elmes` | `this.$message({type: 'success'})` |
|9. | `elmew` | `this.$message({type: 'warning'})` |
|10. | `elmee` | `this.$message({type: 'error'})` |
|11. | `elmei` | `this.$message({type: 'info'})` |
|12. | `elmebox` | `this.$msgbox({})` |
|13. | `elmeal` | `this.$alert({})` |
|14. | `elmecon` | `this.$confirm({})` |
|15. | `elmecons` | `this.$confirm({type: 'success'})` |
|16. | `elmeconw` | `this.$confirm({type: 'warning'})` |
|17. | `elmecone` | `this.$confirm({type: 'error'})` |
|18. | `elmeconi` | `this.$confirm({type: 'info'})` |
|19. | `elmepro` | `this.$prompt({})` |
|20. | `elnoti` | `this.$notify({})` |
|21. | `elnotis` | `this.$notify({type: 'success'})` |
|22. | `elnotiw` | `this.$notify({type: 'warning'})` |
|23. | `elnotie` | `this.$notify({type: 'error'})` |
|24. | `elnotii` | `this.$notify({type: 'info'})` |
|25. |TODO |VNode for Message|


#### Navigation Part
No. |  Trigger Key | Element Tag
|:------:|:--------------:|:--------|
|1. | `elmen` | `<el-menu>` |
|2. | `elsubmen` | `<el-submenu>` |
|3. | `elmeni` | `<el-menu-item>` |
|4. | `eltabs` | `<el-tabs>` |
|5. | `eltabp` | `<el-tab-pane>` |
|6. | `elbr` | `<el-breadcrumb>` |
|7. | `elbri` | `<el-breadcrumb-item>` |
|8. | `eldr` | `<el-dropdown>` |
|9. | `eldri` | `<el-dropdown-item>` |
|10. | `elsts` | `<el-steps>` |
|11. | `elst` | `<el-step>` |

#### Others Part
No. |  Trigger Key | Element Tag
|:------:|:--------------:|:--------|
|1. | `eldi` | `<el-dialog>` |
|2. | `elto` | `<el-tooltip>` |
|3. | `elpop` | `<el-popover>` |
|4. | `elcard` | `<el-card>` |
|5. | `elcaro` | `<el-carousel>` |
|6. | `elcaroi` | `<el-carousel-item>` |
|7. | `elcolla` | `<el-collapse>` |
|8. | `elcollai` | `<el-collapse-item>` |

#### General Part
No. |  Trigger Key | Element Tag
|:------:|:--------------:|:--------|
|1. | `el` | `<el-*>` |
|2. | `elic` | `<el-icon-*>` |

#### Options Part
No. |  Trigger Key | Element Tag
|:------:|:--------------:|:--------|
|1. | `elpos` | positions |
|2. | `elanims` | animation types |

<!--
#### #TODO
1. `tree`的data值
2. `import`样式的快捷方式
3. 不同类型的`button`
4. 各种引用路径：内置动画，样式
-->


