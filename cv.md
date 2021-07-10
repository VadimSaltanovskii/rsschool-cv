# Curriculum vitae

1. **Name:** Vadim Saltanovskii
2. **Location:** Moscow, Russia
3. **Contacts:** 
   - Tel: +7 901-283-11-88
   - Telegram: @saltanovskii
   - Email: noobocode@gmail.com
4. **About me:** Hi, my name is Vadim and I am a beginner web developer. A year ago, I became interested in this profession and now I am immersed in it with all of my head. I am looking for a cool team or project where I can apply all my skills and also gain professional and career growth.  
My advantages:  
    - learnability
    - adequacy
5. **Skills:**
    - HTML ★★★☆☆
    - CSS (Scss / Sass) ★★★☆☆
    - JS ES6+ ★★★☆☆
    - TypeScript ★★☆☆☆
    - Git ★★★☆☆
    - ReactJS ★★☆☆☆
    - Redux ★★☆☆☆
    - VueJs ★★☆☆☆
    - Vuex ★★☆☆☆  
    Soft:
    - VS Code ★★★☆☆

6. **Code example:**
    ```
    import { TextField } from '@material-ui/core';
    import React, { ChangeEvent, KeyboardEvent, useState } from 'react';

    export type EditSpanPropsType = {
        title: string
        renameItem: (newItemTitle: string) => void
    }

    export function EditSpan(props: EditSpanPropsType) {

        let [editMode, setEditMode] = useState<boolean>(false)
        let [inputValue, setInputValue] = useState<string>('')

        const activatedEditMode = () => {
            setEditMode(true)
            setInputValue(props.title)
        }
        const activatedViewMode = () => {
            setEditMode(false)
            props.renameItem(inputValue);
        }
        const inputOnChangeHandler = (event: ChangeEvent<HTMLInputElement>) =>      setInputValue(event.currentTarget.value)

        const inputOnKeyPressHandler = (event:      KeyboardEvent<HTMLInputElement>)     => {
            if (event.key === 'Enter') {
                activatedViewMode();
            }
        }

        return (
            editMode ?
                <TextField
                    color={'secondary'}
                    variant={'outlined'}
                    size={'small'}
                    onKeyPress={inputOnKeyPressHandler}
                    type="text"
                    value={inputValue}
                    onDoubleClick={activatedViewMode}
                    onBlur={activatedViewMode}
                    autoFocus
                    onChange={inputOnChangeHandler} /> :
                <span
                    onDoubleClick={activatedEditMode}>{props.title}</span>
        )
    }
    ```
7. **Job experiense:**
   - Elbrus coding bootcamp 06.2020 - 09.2020  
    Moscow, Russia  
    Fullstack developer  
    Projects:  
        - [Risk app](https://github.com/romaperlos/risk)
    - Kama Games Studio 02.2021 - present  
    Moscow, Russia  
    Junior fullstack developer  
    1. Stack:  
        - HTML
        - CSS
        - JS
        - PHP
        - VueJS
        - SQL
        - MongoDB

    2. Responsibilities:
        - Development and maintenance of company websites
7. **Education:**
    - Donetsk National Technical University (DonNTU) 2007 - 2012  
        Faculty: Economics and Management  
        Specialty: Management of organizations  
        Specialist degree
    - Elbrus Coding Bootcamp 2020  
        Fullstack developer
8. **English:** B1
