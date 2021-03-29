# useForm

Example:

```
    import { useForm } from '../../hooks/useForm';
    
    const [formValues, handleInputChange, reset] = useForm({
        email: 'kevksar@gmail.com',
        password: '12345',
    });

    const { email, password } = formValues;
    
    
    <input           
        name='email'
        value={email}
        onChange={handleInputChange}
    />
    <input
        name='password'
        value={password}
        onChange={handleInputChange}
    />

```




/* 
Usage:
1- Import "useForm".
2- Create >>> 
    const[formValues, handleInputChange] = useForm({
        (NAME OF INPUT): '',   <<<<<  initial values
        (NAME OF INPUT): ''    <<<<<  initial values
    }).
3- Use the desctructuring >>>
    const{NAME OF INPUT, NAME OF INPUT} = formValues
4- Add the (name='NAME OF INPUT') to the inputs.
5- Use the "reset()" to restore the initial value and clean up the input
*/
