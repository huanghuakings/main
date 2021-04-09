# redux
## redux-toolkit

* import {createSlice} from '@reduxjs/toolkit'

const UserInfoModel = createSlice({
    name:"userInfo",
    initialState:INIT_STATE,
    reducers:{
        updateName(state,action){
            state.name = action.payload
        },
        updateAge(state,action){
            state.age = action.payload
        }
    }
})

// 获取reducer 、 action
const {actions,reducer} = UserInfoModel

// 导出action
export const {updateName,updateAge} = actions
// 导出reducer
export const UserInfo = reducer

作者：hboot
链接：https://juejin.cn/post/6927665767651966990
来源：掘金
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。
