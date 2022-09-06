<script>
    export let status = 'valid'
    export let textButton = `Post has been ${status} !`;
    export let alertType = 'valid'
      
    </script>
    <style>
     
    .valid {
      background-color: #78c67b;
      border: solid 2px #1e5d20;
      border-radius: 10px;
      color: #1e5d20;
      font-weight: 600;
      padding: 20px 50px;
    }
    .archived {
      background-color: #c89658;
      border: solid 2px #86591e;
      border-radius: 10px;
      color: #86591e;
      font-weight: 600;
      padding: 20px 50px;

    }
    .deleted {
      background-color: #c85858;
      border: solid 2px #861e1e;
      border-radius: 10px;
      color: #861e1e;
      font-weight: 600;
      padding: 20px 50px;

    }
    .updated {
      background-color: #789cc6;
      border: solid 2px #1e325d;
      border-radius: 10px;
      color: #1e325d;
      font-weight: 600;
      padding: 20px 50px;
    }
    
    </style>
    
    <div class={alertType}> 
        { textButton } 
    </div>
    
    