export const storeName = {
  namespaced: true,
  
  state: {
    dataList: [],
    dataCount: null
  },
  
  mutations: {
    setData (state, payload) {
      state.dataList = payload.dataList || []
      state.dataCount = payload.dataCount || 0
    }
  },
  
  actions: {
    loadData ({ commit }, payload) {
      if (payload) {
        commit('setData', payload)
      } else {
        console.error('Cannot set in loadData')
      }
    }
  },
  
  getters: {
    getFirstInList: (state) => state.dataList && state.dataList[0],
    getDoubleCount: (state) => state.dataCount * 2
  }
}
