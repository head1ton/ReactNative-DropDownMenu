
# react-native-dropdownmenu

## Getting started

`$ npm install react-native-dropdownmenu --save`

### Mostly automatic installation

`$ react-native link react-native-dropdownmenu`


## Usage
```javascript
import Dropdownmenu from 'react-native-dropdownmenu';
let conditionData = [["one", "tow", "three"], ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"],
                        ["Java", "PHP", "C#", "JS", "C++", "Python"]];
<DropdownMenu
                style={{flex: 1}}
                bgColor={'white'}
                tintColor={'#666666'}
                activityTintColor={'green'}
                // arrowImg={}
                // checkImage={}
                // optionTextStyle={{color: '#333333'}}
                // titleStyle={{color: '#333333'}}
                maxHeight={300}
                handler={(selection, row) =>
                    // this.setState({text: data[selection][row]})
                    this._conditionChange(selection,row)
                }
                data={conditionData}
                selectIndex={[0,2,0]}>
                
</DropdownMenu>
```

  