
#  :heavy_check_mark: Desafio 03 - React Native 

Neste desafio completa e fecha a primeira semana do Bootcamp - com a criação de uma aplicação mobile super simples, porém que aplica vários conceitos fundamentais do React Native.

## O que é o ReactJS

- Uma ver são de React para  desenvolvimento Mobile
- Multiplataforma
- Permite manipular cada plataforma de forma diferente

## Sintaxe

- Não utiliza HTML, apenas componentes próprios
- Aplica estilo sem classes os ID´s

Exemplo de componente e stylo 

```
Import {
	StyleSheet,
	View,
	Text,
	TouchableOpacity
} from 'react-native';

function Button(){
	return(
		<View style ={styles.container}>
			<TouchableOpacity style={styles.button}>
				<Text style={styles.text}>Enviar</Text>
			 </TouchableOpacity>
		</View>
	);
}

//Exemplo de Styles

const styles = StyleSheet.create({
	container: {
		alignItems: 'center',
	},
	button : {
			backgroundColor: '#7159c1',	
	},
	text: {
			fontWeight: 'bold',
	}
});
```

### Axios

Algumas opções para utilizar e  conectar o emulador com o backend em Node.js

> ### baseUrl Com Android: 
> - Com emulador do Android Studio: 
> ``` adb reverse tcp:3333 tcp:333 ```
> - ou o ip 10.0.2.2 
> - Com dispositivo fisico: 
>- ip da maquina que roda o backend em node.js

#  :pushpin: O DESAFIO: 
a aplicação que armazena repositórios do portfólio, que utiliza o  backend  em Node.js do 1º desafio.
