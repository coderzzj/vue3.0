###  v-model 用法
### 1.基本用法
##  默认情况下，组件上的 v-model 使用 modelValue 作为 prop 和 update:modelValue 作为事件

# 1. props中定义从父组件传入的值 例如：title

# 2.将props中值 绑定到 :value="title"

# 3.emits [] 中定义要 发射到父组件的事件 "update:title"
# 4. @imput="$emit('update:title, $event.target.value')"

## 2.多个v-model绑定--单个组件实例上创建多个 v-model 绑定

# 利用以特定 prop 和 事件 为目标的能力，在一个组件中传人多个props和emits[],我们可以实现多个v-model绑定，将值传人props

## 3.内置修饰符---v-model 有内置修饰符——.trim、.number 和 .lazy

# 支持自定义修饰符:对于带参数的 v-model 绑定，生成的 prop 名称将为 arg + "Modifiers"