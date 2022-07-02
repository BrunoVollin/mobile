![image](https://inatel.br/cdghub/images/cdg-hub.jpg)
*  [Documentação React Native](https://reactnative.dev/docs/tutorial)
*  [Inputs React Native](https://reactnative.dev/docs/handling-text-input)
*  [Documentação Flutter](https://docs.flutter.dev/development/ui/widgets-intro)
*  [Slides](https://github.com/BrunoVollin/secomp/blob/master/slides/introducao%20ao%20flutter.pdf)
*  [Material Mobile CDG Hub](https://cookie-submarine-e90.notion.site/Mobile-eb12212247fb42738c82f0d3fe148e03)

```js
import React, { useState } from 'react';
import { Text, TextInput, View, Image } from 'react-native';

const PizzaTranslator = () => {
  const [text, setText] = useState('');
  return (
    <View style={{ padding: 10, display:  'flex', justifyContent: "center", alignItems: "center" }}>
      <Image
        style={{
          height:200,
          width:200
        }}
        source={{
          uri: 'https://neurochispas.com.br/wp-content/uploads/2021/08/formula-para-o-volume-de-um-cubo.png',
        }}
      />
      <TextInput
        style={{ height: 40, backgroundColor: "#cccc", width: "80vw" }}
        placeholder="Entre com a aresta!"
        onChangeText={(newText) => setText(newText)}
        defaultValue={text}
      />
      <Text style={{ padding: 10, fontSize: 42 }}>
      {text * text * text} m^3</Text>
    </View>
  );
};

export default PizzaTranslator;

```
  

