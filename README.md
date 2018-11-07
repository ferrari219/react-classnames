# react-classnames

classnames+cssmodule Tutorial


### How to install

<pre>yarn add node-sass classnames</pre>


### How to use

Cnx.js
<pre>
import React, { Component } from 'react';
import styles from './Cnx.module.scss';
import classNames from 'classnames/bind';

const cx = classNames.bind(styles);

class Cnx extends Component {
    render() {
        return (
            <div className={cx('fs','fw')}>
                test text
            </div>
        );
    }
}

export default Cnx;
</pre>


Cnx.module.scss
<pre>
.fs{
    font-size:20px;
}
.fw{
    font-weight:bold;
}
</pre>
