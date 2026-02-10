# CST8915 Lab 1: Algonquin Pet Store on Azure VM

**Student Name**: Akash Patel
**Student ID**: 041269598
**Course**: CST8915 Full-stack Cloud-native Development
**Semester**: Winter 2026

---

## Demo Video

🎥 I added the video under over here: [Click here](https://drive.google.com/file/d/1Ij304F-K6tpYlryo4Qj2TIRF-bPFGe_r/view?usp=sharing)

---

## Technical Explanations

### Order Service (Node.js)

It is simple node js application where we are connecting to Rabbit MQ and send the message to Queue (order_queue).

### Product Service (Rust)

Product service developed on Rust language and main purpose is to fetch products as we mentioned hard-coded on main.rs. I think for rust configuration file is Cargo.toml where we need to mentioned the packages that we need to use it.

### Store Front (Vue.js)

We have created front-end using Vue.js language and install necessary package to run the application and it mentioned in the package.json. We have App.vue as main file and we render the OrderForm from that file. In OrderForm file we are fetching products using products service and submit the order using order service. 


---

## Challenges and Learnings (Optional)

Learning
- Setup the services on VM.
- Run the different services to understand the workflow.

Challenges
- Permission on .pem file while accessing the VM -It complains that no user can have access on that file.


---

## Acknowledgments

- https://github.com/ramymohamed10/26W_CST8915_Lab1
- https://www.youtube.com/watch?v=5tMGdEtBOrs&t=1s
